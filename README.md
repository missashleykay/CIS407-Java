# CIS407-Java
Strayer Java Programming II

import java.util.Scanner;

public class TriangleArea {
   public static void main(String[] args) {
      Scanner scnr = new Scanner(System.in);
      
      Triangle triangle1 = new Triangle();
      Triangle triangle2 = new Triangle();
      
      triangle1.setBase(scnr.nextDouble());
      triangle1.setHeight(scnr.nextDouble());
      triangle2.setBase(scnr.nextDouble());
      triangle2.setHeight(scnr.nextDouble());
      
      Triangle larger=null;
       // check the condition.
       if(triangle1.getArea()>triangle2.getArea())
       larger=triangle1;
       else
       larger=triangle2;
       // Display the result on console.
       System.out.println("Triangle with larger area:");
       // Call the method.
       larger.printInfo();
     
      
   }
}
