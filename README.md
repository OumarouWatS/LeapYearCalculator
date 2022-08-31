// LeapYearCalculator
// This is a Java coded program that checks if a year is a Leap year or not.

import java.util.Scanner;
import com.sun.source.tree.WhileLoopTree;
class Main {
  // This is the Leap Year Calculator
  public static void main(String[] args) {
    int year;
    String decision;
    System.out.println("Hello world!");
    Scanner scnr = new Scanner(System.in);
    System.out.println("Please, enter the year in order to determine the type:");
    year = scnr.nextInt();
    do {
      if((year%400 == 0 || year%100 == 0) && (year % 4 == 0)){
          System.out.println("The year is a leap year. It has 366 days.");
        } else {
    System.out.println("The year is not a leap year, it has 365 days.");
}
      System.out.println("Do you want to keep checking years? Please, answer by Yes or No");
decision = scnr.nextLine();
} while (decision == "Yes");
    System.out.println("Goodbye!!!");
    scnr.close();
}
}
