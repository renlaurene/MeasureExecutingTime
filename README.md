# MeasureExecutingTime
byUsingJavaMethod to measure executing time
To calculate the time need by (stopTime-startTime)


// $javac TimeTest.java
// $java -Xmx128M -Xms16M TimeTest
// 9746465
public class TimeTest {
   static void test(int n) {
      long total = 0;
      for (int i = 0; i < n; i++) {
         total += i;
      }
   }
   public static void main(String[] args) {
      // Using nanoTime() is more precise
      long startTime = System.nanoTime();
      test(10000000); 
      long stopTime = System.nanoTime();
      System.out.println(stopTime - startTime);
   }
}
