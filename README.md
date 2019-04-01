# MeasureExecutingTime
byUsingJavaMethod to measure executing time
The general idea is to calculate the executing time by (stopTime-startTime)
Souce code is using Java as the following, also exmple code by using python and c are given as reference 


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
