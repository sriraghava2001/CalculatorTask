# calculator task
import java.util.*;
import java.lang.*;
public class Calculator {
   public static void main(String[] args) {
      double n1;
      double n2;
      double result;
      int num;
      Scanner in = new Scanner(System.in);
      System.out.println("Enter two numbers: ");
      n1 = in.nextDouble();
      n2 = in.nextDouble();
      System.out.println("Enter a number 1(add) 2(subtract) 3(multiply) 4(divide) ");
      num = in.nextInt();
      switch(num) {
         case 1: result = add(n1,n2);
                 System.out.println("The addition is :");
                 System.out.println(result);
            break;
         case 2: result = sub(n1,n2);
                 System.out.println("The subtraction is :");
                 System.out.println(result);
            break;
         case 3: result = mul(n1,n2);
                 System.out.println("The multiplication  is :");
                 System.out.println(result);
            break;
         case 4: result = div(n1,n2);
                 System.out.println("The division is :");
                 System.out.println(result);
            break;
            default: System.out.println("Error! Enter correct number(1,2,3,4)");
      }
   }
   public static double add(double a,double b){
       return a+b;
   }
   public static double sub(double a,double b){
       return a-b;
   }
   public static double mul(double a,double b){
       return a*b;
   }
   public static double div(double a,double b){
       return a/b;
   }
}
