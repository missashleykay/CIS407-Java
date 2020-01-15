# CIS407-Java
Strayer Java Programming II lab 1.20

import java.util.Scanner;

import java.util.Scanner;

class FoodItem {
private String name;
private double fat;
private double carbs;
private double protein;

// TODO: Define default constructor
FoodItem()
{
this.name="None";
this.fat=0.0;
this.carbs=0.0;
this.protein=0.0;
  
}
FoodItem(String name,double fat,double carbs,double protein)
{
this.name=name;
this.fat=fat;
this.carbs=carbs;
this.protein=protein;
  
}

// TODO: Define second constructor with arguments to initialize
// private fields (name, fat, carbs, protein)

public String getName() {
return name;
}

public double getFat() {
return fat;
}

public double getCarbs() {
return carbs;
}

public double getProtein() {
return protein;
}

public double getCalories(double numServings) {
// Calorie formula
double calories = ((fat * 9) + (carbs * 4) + (protein * 4)) * numServings;
return calories;
}

public void printInfo() {
System.out.println("Nutritional information per serving of " + name + ":");
System.out.println(" Fat: " + fat + "g");
       System.out.println(" Carbohydrates: " + carbs + "g");
       System.out.println(" Protein: " + protein + "g");
}
}
