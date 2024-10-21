# Day 1 Assignment - MLSA Java Workshop

This repository contains the solution to 5 basic programming assignments covered in **Day 1** of the **Microsoft Learn Student Ambassador (MLSA)** workshop. The codes are written in **Java** and cover foundational concepts like area calculation, multiplication tables, factorials, grade checking, and leap year determination.

## Table of Contents
1. [Assignment 1 - Area of a Rectangle](#assignment-1---area-of-a-rectangle)
2. [Assignment 2 - Multiplication Table](#assignment-2---multiplication-table)
3. [Assignment 3 - Factorial of a Number](#assignment-3---factorial-of-a-number)
4. [Assignment 4 - Grade Checker](#assignment-4---grade-checker)
5. [Assignment 5 - Leap Year Checker](#assignment-5---leap-year-checker)

---

## Assignment 1 - Area of a Rectangle
This program calculates the **area of a rectangle** based on user input for length and width.

- **Concepts Used**: Input handling, basic arithmetic operations.
- **Input**: Length and width of the rectangle.
- **Output**: The calculated area of the rectangle.

### Code:
```java
import java.util.Scanner;

public class AreaOfRectangle {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Input: Length and width
        System.out.print("Enter the length of the rectangle: ");
        double length = scanner.nextDouble();
        
        System.out.print("Enter the width of the rectangle: ");
        double width = scanner.nextDouble();
        
        // Calculate the area
        double area = length * width;
        
        // Output the result
        System.out.println("The area of the rectangle is: " + area);
    }
}
```

---

## Assignment 2 - Multiplication Table
This program prints the **multiplication table** for a number up to 10.

- **Concepts Used**: Loops, arithmetic operations.
- **Input**: An integer number.
- **Output**: The multiplication table for that number up to 10.

### Code:
```java
import java.util.Scanner;

public class MultiplicationTable {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Input: An integer number
        System.out.print("Enter a number: ");
        int num = scanner.nextInt();
        
        // Generate multiplication table up to 10
        for (int i = 1; i <= 10; i++) {
            System.out.println(num + " x " + i + " = " + num * i);
        }
    }
}
```

---

## Assignment 3 - Factorial of a Number
This program calculates the **factorial** of a number using a `for` loop.

- **Concepts Used**: Loops, arithmetic operations.
- **Input**: An integer number.
- **Output**: The factorial of the given number.

### Code:
```java
import java.util.Scanner;

public class FactorialOfNumber {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Input: A number
        System.out.print("Enter a number: ");
        int num = scanner.nextInt();
        
        int factorial = 1;
        
        // Calculate factorial using a for loop
        for (int i = 1; i <= num; i++) {
            factorial *= i;
        }
        
        // Output the result
        System.out.println("The factorial of " + num + " is: " + factorial);
    }
}
```

---

## Assignment 4 - Grade Checker
This program checks and prints the **grade** based on a score between 0 and 100.

- **Concepts Used**: Conditional statements.
- **Input**: A score (0-100).
- **Output**: The corresponding grade (A-F).

### Code:
```java
import java.util.Scanner;

public class GradeChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Input: Score (0-100)
        System.out.print("Enter the score (0-100): ");
        int score = scanner.nextInt();
        char grade;
        
        // Check grade based on the score
        if (score >= 90) {
            grade = 'A';
        } else if (score >= 80) {
            grade = 'B';
        } else if (score >= 70) {
            grade = 'C';
        } else if (score >= 60) {
            grade = 'D';
        } else {
            grade = 'F';
        }
        
        // Output the grade
        System.out.println("The grade is: " + grade);
    }
}
```

---

## Assignment 5 - Leap Year Checker
This program checks whether a given year is a **leap year** or not.

- **Concepts Used**: Conditional statements, modulo arithmetic.
- **Input**: A year.
- **Output**: Whether the year is a leap year or not.

### Code:
```java
import java.util.Scanner;

public class LeapYearChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Input: A year
        System.out.print("Enter a year: ");
        int year = scanner.nextInt();
        
        // Check if it's a leap year
        boolean isLeapYear;
        if (year % 4 == 0) {
            if (year % 100 == 0) {
                isLeapYear = year % 400 == 0;
            } else {
                isLeapYear = true;
            }
        } else {
            isLeapYear = false;
        }
        
        // Output the result
        if (isLeapYear) {
            System.out.println(year + " is a leap year.");
        } else {
            System.out.println(year + " is not a leap year.");
        }
    }
}
```

---

## How to Run the Programs

1. Clone this repository to your local machine:
   ```bash
   git clone https://github.com/your-username/day1-mlsa-assignments.git
   ```
   
2. Navigate to the project directory:
   ```bash
   cd day1-mlsa-assignments
   ```

3. Compile and run any of the Java programs using a terminal:
   ```bash
   javac ProgramName.java
   java ProgramName
   ```

   Replace `ProgramName` with the name of the file (e.g., `AreaOfRectangle`, `MultiplicationTable`, etc.).

## Conclusion

These assignments aim to strengthen your foundational programming concepts using **Java**. Each program is designed to introduce and reinforce key topics such as conditional logic, loops, and input handling.

Feel free to modify, experiment, and expand upon the provided code. Happy coding!

---

### Author:
- **Chandra Prakash Ojha** - *MLSA Workshop Participant*
