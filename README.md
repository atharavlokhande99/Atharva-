Experiment 1
Problem Statement :-
1. Write a program to input 2 numbers from the user and display their
addition, multiplication, subtraction, and division.
import java.util.Scanner;
public class Main {
public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);
// Read the first number from the user
System.out.print("Enter the first number: ");
int num1 = scanner.nextInt();
// Read the second number from the user
System.out.print("Enter the second number: ");
int num2 = scanner.nextInt();
// Calculate the sum, difference, product, and quotient of the two numbers
int sum = num1 + num2;
int difference = num1 - num2;
int product = num1 * num2;
int quotient = num1 / num2;
// Display the results
System.out.println("The sum of the two numbers is: " + sum);
System.out.println("The difference of the two numbers is: " + difference);
System.out.println("The product of the two numbers is: " + product);
System.out.println("The quotient of the two numbers is: " + quotient);
}
}
Output:-
Enter the first number: 10
Enter the second number: 5
The sum of the two numbers is: 15
The difference of the two numbers is: 5
The product of the two numbers is: 50
The quotient of the two number is: 2
Problem Statement :-
2. Write a program to accept value of marks of 5 subjects and calculate
percentage and display it.
import java.util.Scanner;
public class CalculatePercentage {
public static void main(String[] args) {
Scanner scanner = new Scanner(System.in);
// Get the marks of 5 subjects from the user
System.out.println("Enter the marks of 5 subjects:");
int subject1 = scanner.nextInt();
int subject2 = scanner.nextInt();
int subject3 = scanner.nextInt();
int subject4 = scanner.nextInt();
int subject5 = scanner.nextInt();
// Calculate the total marks
int totalMarks = subject1 + subject2 + subject3 + subject4 + subject5;
// Calculate the percentage
float percentage = (totalMarks / 500.0f) * 100.0f;
// Display the percentage
System.out.println("The percentage is: " + percentage);
}
}
Output:-
Enter the marks of 5 subjects:
90
80
70
60
50
The percentage is: 70.0
Problem Statement :-
3. Write a program to assign value of radius then calculate the area of circle by
using method calling (use arithmetic promotion).
import java.util.Scanner;
public class CircleAreaCalculator {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Prompt the user to enter the radius
 System.out.print("Enter the radius of the circle: ");
 double radius = scanner.nextDouble();
 // Call the method to calculate the area
 double area = calculateArea(radius);
 // Display the result
 System.out.println("The area of the circle with radius " + radius + " is: " +
area);
 }
 // Method to calculate the area of a circle
 private static double calculateArea(double radius) {
 // Formula for the area of a circle: A = π * r^2
 double area = Math.PI * Math.pow(radius, 2);
 return area;
 }
}
Output:-
Enter the radius of the circle: 5
The area of the circle with radius 5.0 is: 78.53981633974483
Problem Statement :-
4. Write a program to calculate area of triangle and area of rectangle by using
method calling.
import java.util.Scanner;
public class AreaCalculator {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Get input for triangle
 System.out.print("Enter the base of the triangle: ");
 double base = scanner.nextDouble();
 System.out.print("Enter the height of the triangle: ");
 double height = scanner.nextDouble();
 // Call the method to calculate the area of the triangle
 double triangleArea = calculateTriangleArea(base, height);
 // Display the result for triangle
 System.out.println("The area of the triangle with base " + base + " and height
" + height + " is: " + triangleArea);
 // Get input for rectangle
 System.out.print("Enter the length of the rectangle: ");
 double length = scanner.nextDouble();
 System.out.print("Enter the width of the rectangle: ");
 double width = scanner.nextDouble();
 // Call the method to calculate the area of the rectangle
 double rectangleArea = calculateRectangleArea(length, width);
 // Display the result for rectangle
 System.out.println("The area of the rectangle with length " + length + " and
width " + width + " is: " + rectangleArea);
 }
 // Method to calculate the area of a triangle
 private static double calculateTriangleArea(double base, double height) {
 // Formula for the area of a triangle: A = 0.5 * base * height
 return 0.5 * base * height;
 }
 // Method to calculate the area of a rectangle
 private static double calculateRectangleArea(double length, double width) {
 // Formula for the area of a rectangle: A = length * width
 return length * width;
 }
}
Output:-
Enter the base of the triangle: 6
Enter the height of the triangle: 8
The area of the triangle with base 6.0 and height 8.0 is: 24.0
Enter the length of the rectangle: 5
Enter the width of the rectangle: 10
The area of the rectangle with length 5.0 and width 10.0 is: 50.0
Experiment No.:
Problem Statement :-
1. Write a program to perform mathematical operations by using different
methods of Math class.
public class MathOperations {
 public static void main(String[] args) {
 // Example values for demonstration
 double number1 = 5.4;
 double number2 = 2.6;
 // Math operations using different methods
 double sum = add(number1, number2);
 double difference = subtract(number1, number2);
 double product = multiply(number1, number2);
 double quotient = divide(number1, number2);
 double power = power(number1, 2); // 5.4^2
 double squareRoot = squareRoot(number2);
 // Display the results
 System.out.println("Sum: " + sum);
 System.out.println("Difference: " + difference);
 System.out.println("Product: " + product);
 System.out.println("Quotient: " + quotient);
 System.out.println("Power: " + power);
 System.out.println("Square Root: " + squareRoot);
 }
 // Method to add two numbers
 private static double add(double a, double b) {
 return Math.addExact((int) a, (int) b); // Example of addExact method
 }
 // Method to subtract two numbers
 private static double subtract(double a, double b) {
 return a - b;
 }
 // Method to multiply two numbers
 private static double multiply(double a, double b) {
 return Math.multiplyExact((int) a, (int) b); // Example of multiplyExact
method
 }
 // Method to divide two numbers
 private static double divide(double a, double b) {
 return a / b;
 }
 // Method to calculate the power of a number
 private static double power(double base, double exponent) {
 return Math.pow(base, exponent);
 }
 // Method to calculate the square root of a number
 private static double squareRoot(double number) {
 return Math.sqrt(number);
 }
}
Output:-
Sum: 8.0
Difference: 2.8
Product: 10.0
Quotient: 2.076923076923077
Power: 29.16
Square Root: 1.61245154965971
Problem Statement :-
2. Write a program to accept the string from the user to perform string
related operations by using different methods of String class.
import java.util.Scanner;
public class UserStringOperations {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accept a string from the user
 System.out.print("Enter a string: ");
 String userInput = scanner.nextLine();
 // Perform string operations using different methods
 int length = userInput.length();
 String upperCase = userInput.toUpperCase();
 String lowerCase = userInput.toLowerCase();
 String trimmedString = userInput.trim();
 boolean startsWithHello = userInput.startsWith("Hello");
 boolean endsWithWorld = userInput.endsWith("World");
 int indexOfLetterO = userInput.indexOf('o');
 String substringFromIndex5 = userInput.substring(5);
 // Display the results
 System.out.println("Length of the string: " + length);
 System.out.println("Uppercase: " + upperCase);
 System.out.println("Lowercase: " + lowerCase);
 System.out.println("Trimmed string: " + trimmedString);
 System.out.println("Starts with 'Hello': " + startsWithHello);
 System.out.println("Ends with 'World': " + endsWithWorld);
 System.out.println("Index of 'o': " + indexOfLetterO);
 System.out.println("Substring from index 5: " + substringFromIndex5);
 }
}
Output:-
Enter a string: Hello, World!
Length of the string: 15
Uppercase: HELLO, WORLD!
Lowercase: hello, world!
Trimmed string: Hello, World!
Starts with 'Hello': true
Ends with 'World': true
Index of 'o': 4
Substring from index 5: , World!
Experiment No.:
Problem Statement :-
1. Write a program to perform addition by changing the number of arguments
using function overloading.
public class AdditionWithOverloading {
 public static void main(String[] args) {
 // Example with two numbers
 int sum1 = add(5, 10);
 System.out.println("Sum 1: " + sum1);
 // Example with three numbers
 int sum2 = add(15, 20, 25);
 System.out.println("Sum 2: " + sum2);
 // Example with four numbers
 int sum3 = add(30, 35, 40, 45);
 System.out.println("Sum 3: " + sum3);
 }
 // Method for adding two numbers
 private static int add(int a, int b) {
 return a + b;
 }
 // Method for adding three numbers
 private static int add(int a, int b, int c) {
 return a + b + c;
 }
 // Method for adding four numbers
 private static int add(int a, int b, int c, int d) {
 return a + b + c + d;
 }
}
Output:-
Sum 1: 15
Sum 2: 60
Sum 3: 150
Problem Statement :-
2. Write a program to perform multiplication by changing the data types using
function overloading.
public class MultiplicationWithOverloading {
 public static void main(String[] args) {
 // Example with two integers
 int result1 = multiply(5, 10);
 System.out.println("Result 1: " + result1);
 // Example with two doubles
 double result2 = multiply(2.5, 3.5);
 System.out.println("Result 2: " + result2);
 // Example with an integer and a double
 double result3 = multiply(4, 1.5);
 System.out.println("Result 3: " + result3);
 }
 // Method for multiplying two integers
 private static int multiply(int a, int b) {
 return a * b;
 }
 // Method for multiplying two doubles
 private static double multiply(double a, double b) {
 return a * b;
 }
 // Method for multiplying an integer and a double
 private static double multiply(int a, double b) {
 return a * b;
 }
}
Output:-
Result 1: 50
Result 2: 8.75
Result 3: 6.0
Problem Statement :-
3. Write a program to declare class student having data member id and name,
initialized it using default constructor for two object of class and display all
records.
public class Student {
 // Data members
 private int id;
 private String name;
 // Default constructor
 public Student() {
 // Default values
 id = 0;
 name = "Unknown";
 }
 // Parameterized constructor
 public Student(int id, String name) {
 this.id = id;
 this.name = name;
 }
 // Method to display student information
 public void displayStudentInfo() {
 System.out.println("Student ID: " + id);
 System.out.println("Student Name: " + name);
 System.out.println();
 }
 public static void main(String[] args) {
 // Create two objects of the Student class using the default constructor
 Student student1 = new Student();
 Student student2 = new Student();
 // Display information for both students
 System.out.println("Student 1 Information:");
 student1.displayStudentInfo();
 System.out.println("Student 2 Information:");
 student2.displayStudentInfo();
 }
}
Output:-
Student 1 Information:
Student ID: 0
Student Name: Unknown
Student 2 Information:
Student ID: 0
Student Name: Unknown
Problem Statement :-
4. Write a program to declare class Book having data member id, name and
price, initialized it using parameterized constructor for two object of class and
display all records.
public class Book {
 // Data members
 private int id;
 private String name;
 private double price;
 // Parameterized constructor
 public Book(int id, String name, double price) {
 this.id = id;
 this.name = name;
 this.price = price;
 }
 // Method to display book information
 public void displayBookInfo() {
 System.out.println("Book ID: " + id);
 System.out.println("Book Name: " + name);
 System.out.println("Book Price: $" + price);
 System.out.println();
 }
 public static void main(String[] args) {
 // Create two objects of the Book class using the parameterized constructor
 Book book1 = new Book(101, "Java Programming", 29.99);
 Book book2 = new Book(102, "Data Structures and Algorithms", 39.99);
 // Display information for both books
 System.out.println("Book 1 Information:");
 book1.displayBookInfo();
 System.out.println("Book 2 Information:");
 book2.displayBookInfo();
 }
}
Output:-
Book 1 Information:
Book ID: 101
Book Name: Java Programming
Book Price: $29.99
Book 2 Information:
Book ID: 102
Book Name: Data Structures and Algorithms
Book Price: $39.99
Problem Statement :-
5. Write a program to declare class Box with data member length, width, height,
initialized three object using different constructors and calculate Volume of Box
and display records.
public class Box {
 // Data members
 private double length;
 private double width;
 private double height;
 // Default constructor
 public Box() {
 // Default values
 length = 1.0;
 width = 1.0;
 height = 1.0;
 }
 // Parameterized constructor with one parameter
 public Box(double side) {
 length = side;
 width = side;
 height = side;
 }
 // Parameterized constructor with three parameters
 public Box(double length, double width, double height) {
 this.length = length;
 this.width = width;
 this.height = height;
 }
 // Method to calculate the volume of the box
 public double calculateVolume() {
 return length * width * height;
 }
 // Method to display box information
 public void displayBoxInfo() {
 System.out.println("Box Dimensions:");
 System.out.println("Length: " + length);
 System.out.println("Width: " + width);
 System.out.println("Height: " + height);
 System.out.println("Volume: " + calculateVolume());
 System.out.println();
 }
 public static void main(String[] args) {
 // Create three objects of the Box class using different constructors
 Box box1 = new Box(); // Default constructor
 Box box2 = new Box(2.5); // Parameterized constructor with one
parameter
 Box box3 = new Box(3.0, 4.0, 5.0); // Parameterized constructor with three
parameters
 // Display information for all three boxes
 System.out.println("Box 1 Information:");
 box1.displayBoxInfo();
 System.out.println("Box 2 Information:");
 box2.displayBoxInfo();
 System.out.println("Box 3 Information:");
 box3.displayBoxInfo();
 }
}
Output:-
Box 1 Information:
Box Dimensions:
Length: 1.0
Width: 1.0
Height: 1.0
Volume: 1.0
Box 2 Information:
Box Dimensions:
Length: 2.5
Width: 2.5
Height: 2.5
Volume: 15.625
Box 3 Information:
Box Dimensions:
Length: 3.0
Width: 4.0
Height: 5.0
Volume: 60.0
Experiment No: - 4 (Control statement)
Problem Statement :-
1. Write a program to accepts three numbers from user and find largest
number.
import java.util.Scanner;
public class FindLargestNumber {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting three numbers from the user
 System.out.print("Enter the first number: ");
 int num1 = scanner.nextInt();
 System.out.print("Enter the second number: ");
 int num2 = scanner.nextInt();
 System.out.print("Enter the third number: ");
 int num3 = scanner.nextInt();
 // Finding the largest number
 int largestNumber = findLargest(num1, num2, num3);
 // Displaying the result
 System.out.println("The largest number is: " + largestNumber);
 // Closing the scanner
 scanner.close();
 }
 // Method to find the largest number among three numbers
 private static int findLargest(int a, int b, int c) {
 if (a >= b && a >= c) {
 return a;
 } else if (b >= a && b >= c) {
 return b;
 } else {
 return c;
 }
 }
}
Output:-
Enter the first number: 25
Enter the second number: 14
Enter the third number: 36
The largest number is: 36
Problem Statement :-
2. Write a program to accept number from user and calculate factorial of given
number.
import java.util.Scanner;
public class FactorialCalculator {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting a number from the user
 System.out.print("Enter a number: ");
 int number = scanner.nextInt();
 // Checking if the number is non-negative
 if (number < 0) {
 System.out.println("Please enter a non-negative number.");
 } else {
 // Calculating factorial
 long factorial = calculateFactorial(number);
 // Displaying the result
 System.out.println("The factorial of " + number + " is: " + factorial);
 }
 // Closing the scanner
 scanner.close();
 }
 // Method to calculate factorial of a number
 private static long calculateFactorial(int n) {
 if (n == 0 || n == 1) {
 return 1;
 } else {
 return n * calculateFactorial(n - 1);
 }
 }
}
Output:-
Enter a number: 5
The factorial of 5 is: 120
Problem Statement :-
3. Write a program to accept number from user and check number is palindrome
or not.
import java.util.Scanner;
public class PalindromeChecker {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting a number from the user
 System.out.print("Enter a number: ");
 int number = scanner.nextInt();
 // Checking if the number is a palindrome
 if (isPalindrome(number)) {
 System.out.println(number + " is a palindrome.");
 } else {
 System.out.println(number + " is not a palindrome.");
 }
 // Closing the scanner
 scanner.close();
 }
 // Method to check if a number is a palindrome
 private static boolean isPalindrome(int n) {
 int originalNumber = n;
 int reversedNumber = 0;
 while (n > 0) {
 int digit = n % 10;
 reversedNumber = reversedNumber * 10 + digit;
 n /= 10;
 }
 return originalNumber == reversedNumber;
 }
}
Output:-
Enter a number: 121
121 is a palindrome.
Problem Statement :-
4. Write a program to accept number from user and check number is
Armstrong or not.
import java.util.Scanner;
public class ArmstrongNumberChecker {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting a number from the user
 System.out.print("Enter a number: ");
 int number = scanner.nextInt();
 // Checking if the number is an Armstrong number
 if (isArmstrongNumber(number)) {
 System.out.println(number + " is an Armstrong number.");
 } else {
 System.out.println(number + " is not an Armstrong number.");
 }
 // Closing the scanner
 scanner.close();
 }
 // Method to check if a number is an Armstrong number
 private static boolean isArmstrongNumber(int n) {
 int originalNumber = n;
 int numberOfDigits = countDigits(n);
 int sum = 0;
 while (n > 0) {
 int digit = n % 10;
 sum += Math.pow(digit, numberOfDigits);
 n /= 10;
 }
 return originalNumber == sum;
 }
 // Method to count the number of digits in a number
 private static int countDigits(int n) {
 int count = 0;
 while (n > 0) {
 n /= 10;
 count++;
 }
 return count;
 }
}
Output:-
Enter a number: 153
153 is an Armstrong number.
Problem Statement :-
5. Write a program to accept number from user and check number is prime or
not.
import java.util.Scanner;
public class PrimeNumberChecker {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting a number from the user
 System.out.print("Enter a number: ");
 int number = scanner.nextInt();
 // Checking if the number is a prime number
 if (isPrime(number)) {
 System.out.println(number + " is a prime number.");
 } else {
 System.out.println(number + " is not a prime number.");
 }
 // Closing the scanner
 scanner.close();
 }
 // Method to check if a number is a prime number
 private static boolean isPrime(int n) {
 if (n <= 1) {
 return false;
 }
 for (int i = 2; i <= Math.sqrt(n); i++) {
 if (n % i == 0) {
 return false;
 }
 }
 return true;
 }
}
Output:-
Enter a number: 17
17 is a prime number.
Experiment No: - 5 (Array)
Problem Statement :-
1. Write a program to accepts ‘n’ number from user to store in array and finds
largest number in an array.
import java.util.Scanner;
public class FindLargestInArray {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting the number of elements in the array
 System.out.print("Enter the number of elements: ");
 int n = scanner.nextInt();
 // Creating an array to store the numbers
 int[] numbers = new int[n];
 // Accepting 'n' numbers from the user and storing them in the array
 for (int i = 0; i < n; i++) {
 System.out.print("Enter element " + (i + 1) + ": ");
 numbers[i] = scanner.nextInt();
 }
 // Finding the largest number in the array
 int largestNumber = findLargestInArray(numbers);
 // Displaying the entered array
 System.out.print("Entered array: ");
 displayArray(numbers);
 // Displaying the result
 System.out.println("The largest number in the array is: " + largestNumber);
 // Closing the scanner
 scanner.close();
 }
 // Method to find the largest number in an array
 private static int findLargestInArray(int[] arr) {
 if (arr.length == 0) {
 throw new IllegalArgumentException("Array is empty");
 }
 int max = arr[0];
 for (int i = 1; i < arr.length; i++) {
 if (arr[i] > max) {
 max = arr[i];
 }
 }
 return max;
 }
 // Method to display the elements of an array
 private static void displayArray(int[] arr) {
 System.out.print("[");
 for (int i = 0; i < arr.length; i++) {
 System.out.print(arr[i]);
 if (i < arr.length - 1) {
 System.out.print(", ");
 }
 }
 System.out.println("]");
 }
}
Output:-
Enter the number of elements: 5
Enter element 1: 14
Enter element 2: 8
Enter element 3: 25
Enter element 4: 10
Enter element 5: 19
Entered array: [14, 8, 25, 10, 19]
The largest number in the array is: 25
Problem Statement :-
2.Write a program accept ‘n’ number storein array and perform linear search.
import java.util.Scanner;
public class LinearSearch {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting the number of elements in the array
 System.out.print("Enter the number of elements: ");
 int n = scanner.nextInt();
 // Creating an array to store the numbers
 int[] numbers = new int[n];
 // Accepting 'n' numbers from the user and storing them in the array
 for (int i = 0; i < n; i++) {
 System.out.print("Enter element " + (i + 1) + ": ");
 numbers[i] = scanner.nextInt();
 }
 // Accepting the number to search
 System.out.print("Enter the number to search: ");
 int searchNumber = scanner.nextInt();
 // Performing linear search
 int index = linearSearch(numbers, searchNumber);
 // Displaying the entered array
 System.out.print("Entered array: ");
 displayArray(numbers);
 // Displaying the result of linear search
 if (index != -1) {
 System.out.println(searchNumber + " found at index " + index + ".");
 } else {
 System.out.println(searchNumber + " not found in the array.");
 }
 // Closing the scanner
 scanner.close();
 }
 // Method to perform linear search in an array
 private static int linearSearch(int[] arr, int target) {
 for (int i = 0; i < arr.length; i++) {
 if (arr[i] == target) {
 return i; // Return the index if the target is found
 }
 }
 return -1; // Return -1 if the target is not found
 }
 // Method to display the elements of an array
 private static void displayArray(int[] arr) {
 System.out.print("[");
 for (int i = 0; i < arr.length; i++) {
 System.out.print(arr[i]);
 if (i < arr.length - 1) {
 System.out.print(", ");
 }
 }
 System.out.println("]");
 }
}
Output:-
Enter the number of elements: 7
Enter element 1: 10
Enter element 2: 24
Enter element 3: 7
Enter element 4: 15
Enter element 5: 32
Enter element 6: 18
Enter element 7: 5
Enter the number to search: 15
Entered array: [10, 24, 7, 15, 32, 18, 5]
15 found at index 3.
Problem Statement :-
3. Write a program to accept 3x3 Matrix and calculate addition of two matrix and
display it.
import java.util.Scanner;
public class MatrixAddition {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting the elements of the first matrix
 int[][] matrix1 = new int[3][3];
 System.out.println("Enter elements for the first matrix (3x3):");
 enterMatrixElements(scanner, matrix1);
 // Accepting the elements of the second matrix
 int[][] matrix2 = new int[3][3];
 System.out.println("Enter elements for the second matrix (3x3):");
 enterMatrixElements(scanner, matrix2);
 // Calculating the sum of the matrices
 int[][] resultMatrix = addMatrices(matrix1, matrix2);
 // Displaying the entered matrices
 System.out.println("First Matrix:");
 displayMatrix(matrix1);
 System.out.println("Second Matrix:");
 displayMatrix(matrix2);
 // Displaying the result of matrix addition
 System.out.println("Sum of the Matrices:");
 displayMatrix(resultMatrix);
 // Closing the scanner
 scanner.close();
 }
 // Method to accept elements for a matrix
 private static void enterMatrixElements(Scanner scanner, int[][] matrix) {
 for (int i = 0; i < matrix.length; i++) {
 for (int j = 0; j < matrix[0].length; j++) {
 System.out.print("Enter element at position (" + (i + 1) + ", " + (j + 1) + "):
");
 matrix[i][j] = scanner.nextInt();
 }
 }
 }
 // Method to add two matrices
 private static int[][] addMatrices(int[][] matrix1, int[][] matrix2) {
 int[][] resultMatrix = new int[3][3];
 for (int i = 0; i < matrix1.length; i++) {
 for (int j = 0; j < matrix1[0].length; j++) {
 resultMatrix[i][j] = matrix1[i][j] + matrix2[i][j];
 }
 }
 return resultMatrix;
 }
 // Method to display a matrix
 private static void displayMatrix(int[][] matrix) {
 for (int i = 0; i < matrix.length; i++) {
 for (int j = 0; j < matrix[0].length; j++) {
 System.out.print(matrix[i][j] + "\t");
 }
 System.out.println();
 }
 System.out.println();
 }
}
Output:-
Enter elements for the first matrix (3x3):
Enter element at position (1, 1): 1
Enter element at position (1, 2): 2
Enter element at position (1, 3): 3
Enter element at position (2, 1): 4
Enter element at position (2, 2): 5
Enter element at position (2, 3): 6
Enter element at position (3, 1): 7
Enter element at position (3, 2): 8
Enter element at position (3, 3): 9
Enter elements for the second matrix (3x3):
Enter element at position (1, 1): 9
Enter element at position (1, 2): 8
Enter element at position (1, 3): 7
Enter element at position (2, 1): 6
Enter element at position (2, 2): 5
Enter element at position (2, 3): 4
Enter element at position (3, 1): 3
Enter element at position (3, 2): 2
Enter element at position (3, 3): 1
First Matrix:
1 2 3
4 5 6
7 8 9
Second Matrix:
9 8 7
6 5 4
3 2 1
Sum of the Matrices:
10 10 10
10 10 10
10 10 10
Problem Statement :-
4. Write a program to declare class Employee having data member empid, name
and salary. Accept records for 5 employee and display that records whose salary
is greater than 5000.
import java.util.Scanner;
class Employee {
 int empid;
 String name;
 double salary;
 // Parameterized constructor
 public Employee(int empid, String name, double salary) {
 this.empid = empid;
 this.name = name;
 this.salary = salary;
 }
}
public class EmployeeRecords {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Creating an array to store Employee objects
 Employee[] employees = new Employee[5];
 // Accepting records for 5 employees
 for (int i = 0; i < employees.length; i++) {
 System.out.println("Enter details for Employee " + (i + 1) + ":");
 System.out.print("Employee ID: ");
 int empid = scanner.nextInt();
 scanner.nextLine(); // Consume the newline character
 System.out.print("Name: ");
 String name = scanner.nextLine();
 System.out.print("Salary: ");
 double salary = scanner.nextDouble();
 // Creating an Employee object and storing it in the array
 employees[i] = new Employee(empid, name, salary);
 }
 // Displaying records of employees with salary greater than 5000
 System.out.println("\nEmployee records with salary greater than 5000:");
 displayRecordsWithSalaryGreaterThan5000(employees);
 // Closing the scanner
 scanner.close();
 }
 // Method to display employee records with salary greater than 5000
 private static void displayRecordsWithSalaryGreaterThan5000(Employee[]
employees) {
 for (Employee employee : employees) {
 if (employee.salary > 5000) {
 System.out.println("Employee ID: " + employee.empid);
 System.out.println("Name: " + employee.name);
 System.out.println("Salary: " + employee.salary);
 System.out.println("----------------------");
 }
 }
 }
}
Output:-
Enter details for Employee 1:
Employee ID: 101
Name: John Doe
Salary: 6000
Enter details for Employee 2:
Employee ID: 102
Name: Jane Doe
Salary: 4500
Enter details for Employee 3:
Employee ID: 103
Name: Mark Smith
Salary: 7000
Enter details for Employee 4:
Employee ID: 104
Name: Emily Johnson
Salary: 5500
Enter details for Employee 5:
Employee ID: 105
Name: Michael Brown
Salary: 4800
Employee records with salary greater than 5000:
Employee ID: 101
Name: John Doe
Salary: 6000
----------------------
Employee ID: 103
Name: Mark Smith
Salary: 7000
----------------------
Employee ID: 104
Name: Emily Johnson
Salary: 5500
----------------------
Problem Statement :-
5. Write a program to declare class Product having data member id, name, price
accepts records for 5 products and display all records and also display total price
of products.
import java.util.Scanner;
class Product {
 int id;
 String name;
 double price;
 // Parameterized constructor
 public Product(int id, String name, double price) {
 this.id = id;
 this.name = name;
 this.price = price;
 }
}
public class ProductRecords {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Creating an array to store Product objects
 Product[] products = new Product[5];
 // Accepting records for 5 products
 for (int i = 0; i < products.length; i++) {
 System.out.println("Enter details for Product " + (i + 1) + ":");
 System.out.print("Product ID: ");
 int id = scanner.nextInt();
 scanner.nextLine(); // Consume the newline character
 System.out.print("Name: ");
 String name = scanner.nextLine();
 System.out.print("Price: ");
 double price = scanner.nextDouble();
 // Creating a Product object and storing it in the array
 products[i] = new Product(id, name, price);
 }
 // Displaying all product records
 System.out.println("\nAll Product records:");
 displayAllProductRecords(products);
 // Calculating and displaying the total price of products
 double totalPrice = calculateTotalPrice(products);
 System.out.println("\nTotal Price of Products: " + totalPrice);
 // Closing the scanner
 scanner.close();
 }
 // Method to display all product records
 private static void displayAllProductRecords(Product[] products) {
 for (Product product : products) {
 System.out.println("Product ID: " + product.id);
 System.out.println("Name: " + product.name);
 System.out.println("Price: " + product.price);
 System.out.println("----------------------");
 }
 }
 // Method to calculate the total price of products
 private static double calculateTotalPrice(Product[] products) {
 double total = 0;
 for (Product product : products) {
 total += product.price;
 }
 return total;
 }
}
Output:-
Enter details for Product 1:
Product ID: 101
Name: Laptop
Price: 1200.50
Enter details for Product 2:
Product ID: 102
Name: Smartphone
Price: 699.99
Enter details for Product 3:
Product ID: 103
Name: Camera
Price: 399.95
Enter details for Product 4:
Product ID: 104
Name: Headphones
Price: 89.99
Enter details for Product 5:
Product ID: 105
Name: Smartwatch
Price: 199.50
All Product records:
Product ID: 101
Name: Laptop
Price: 1200.5
----------------------
Product ID: 102
Name: Smartphone
Price: 699.99
----------------------
Product ID: 103
Name: Camera
Price: 399.95
----------------------
Product ID: 104
Name: Headphones
Price: 89.99
----------------------
Product ID: 105
Name: Smartwatch
Price: 199.5
----------------------
Total Price of Products: 2589.93

Experiment No:- 6 (Inheritance)
Problem Statement :-
1. Write a program to implement following inheritance. Assume suitable
methods.
Superclass
 Class Name: Student
 Member variables: Roll_no, Name
Subclass:
 Class Name: Library
 Member variables: Member_No
import java.util.Scanner;
// Superclass
class Student {
 // Member variables
 int rollNo;
 String name;
 // Parameterized constructor
 public Student(int rollNo, String name) {
 this.rollNo = rollNo;
 this.name = name;
 }
 // Display method to show details of the student
 public void displayStudentDetails() {
 System.out.println("Student Details:");
 System.out.println("Roll No: " + rollNo);
 System.out.println("Name: " + name);
 }
}
// Subclass
class Library extends Student {
 // Additional member variable for the Library subclass
 int memberNo;
 // Parameterized constructor for the Library subclass
 public Library(int rollNo, String name, int memberNo) {
 // Calling the constructor of the superclass (Student)
 super(rollNo, name);
 this.memberNo = memberNo;
 }
 // Display method to show details of the student and library membership
 public void displayLibraryDetails() {
 // Calling the display method of the superclass (Student)
 displayStudentDetails();
 System.out.println("Library Member No: " + memberNo);
 }
}
public class InheritanceExample {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting details for a student
 System.out.print("Enter Student Roll No: ");
 int rollNo = scanner.nextInt();
 scanner.nextLine(); // Consume the newline character
 System.out.print("Enter Student Name: ");
 String name = scanner.nextLine();
 // Accepting library membership details
 System.out.print("Enter Library Member No: ");
 int memberNo = scanner.nextInt();
 // Creating an object of the Library subclass
 Library libraryMember = new Library(rollNo, name, memberNo);
 // Displaying details using the method of the subclass
 libraryMember.displayLibraryDetails();
 // Closing the scanner
 scanner.close();
 }
}
Output:-
Enter Student Roll No: 101
Enter Student Name: John Doe
Enter Library Member No: 5678
Student Details:
Roll No: 101
Name: John Doe
Library Member No: 5678
Problem Statement :-
2. Write a program to implement following multilevel inheritance. Assume
suitable methods.
 a. Class Name: Student
 Member variables: Roll_no, Name
 b. Class Name: Marks
 Member variables: Marks1, Marks2, Total
 c. Class Name: Result
 Member variables: Percentage
import java.util.Scanner;
// Base class
class Student {
 // Member variables
 int rollNo;
 String name;
 // Parameterized constructor
 public Student(int rollNo, String name) {
 this.rollNo = rollNo;
 this.name = name;
 }
 // Display method to show details of the student
 public void displayStudentDetails() {
 System.out.println("Student Details:");
 System.out.println("Roll No: " + rollNo);
 System.out.println("Name: " + name);
 }
}
// Derived class 1
class Marks extends Student {
 // Member variables
 int marks1;
 int marks2;
 int total;
 // Parameterized constructor
 public Marks(int rollNo, String name, int marks1, int marks2) {
 // Calling the constructor of the base class (Student)
 super(rollNo, name);
 this.marks1 = marks1;
 this.marks2 = marks2;
 this.total = marks1 + marks2;
 }
 // Display method to show details of the student and marks
 public void displayMarksDetails() {
 // Calling the display method of the base class (Student)
 displayStudentDetails();
 System.out.println("Marks Details:");
 System.out.println("Marks 1: " + marks1);
 System.out.println("Marks 2: " + marks2);
 System.out.println("Total Marks: " + total);
 }
}
// Derived class 2
class Result extends Marks {
 // Member variable
 double percentage;
 // Parameterized constructor
 public Result(int rollNo, String name, int marks1, int marks2) {
 // Calling the constructor of the intermediate class (Marks)
 super(rollNo, name, marks1, marks2);
 this.percentage = calculatePercentage();
 }
 // Method to calculate percentage
 private double calculatePercentage() {
 return (double) super.total / 2; // Assuming total marks out of 100
 }
 // Display method to show details of the student, marks, and result
 public void displayResultDetails() {
 // Calling the display method of the intermediate class (Marks)
 displayMarksDetails();
 System.out.println("Result Details:");
 System.out.println("Percentage: " + percentage + "%");
 }
}
public class MultilevelInheritanceExample {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting details for a student
 System.out.print("Enter Student Roll No: ");
 int rollNo = scanner.nextInt();
 scanner.nextLine(); // Consume the newline character
 System.out.print("Enter Student Name: ");
 String name = scanner.nextLine();
 // Accepting marks details
 System.out.print("Enter Marks 1: ");
 int marks1 = scanner.nextInt();
 System.out.print("Enter Marks 2: ");
 int marks2 = scanner.nextInt();
 // Creating an object of the Result class
 Result studentResult = new Result(rollNo, name, marks1, marks2);
 // Displaying details using the method of the Result class
 studentResult.displayResultDetails();
 // Closing the scanner
 scanner.close();
 }
}
Output:-
Enter Student Roll No: 101
Enter Student Name: John Doe
Enter Marks 1: 75
Enter Marks 2: 85
Student Details:
Roll No: 101
Name: John Doe
Marks Details:
Marks 1: 75
Marks 2: 85
Total Marks: 160
Result Details:
Percentage: 80.0%
Experiment No:- 7 (Polymorphism)
Problem Statement :-
1. Write a Java program to create a base class Bank with method with
interest_rate(). Create two subclasses SBI and ICICI. Override the
interest_rate () method to find out interest rate.
import java.util.Scanner;
// Base class
class Bank {
 // Method to calculate interest rate (dummy implementation in the base class)
 public void interest_rate() {
 System.out.println("Interest Rate in the Bank class: 4%");
 }
}
// Subclass 1
class SBI extends Bank {
 // Overriding the interest_rate() method in SBI subclass
 @Override
 public void interest_rate() {
 System.out.println("Interest Rate in SBI: 5%");
 }
}
// Subclass 2
class ICICI extends Bank {
 // Overriding the interest_rate() method in ICICI subclass
 @Override
 public void interest_rate() {
 System.out.println("Interest Rate in ICICI: 6%");
 }
}
public class BankExample {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Creating objects of the subclasses
 Bank bank = new Bank();
 SBI sbi = new SBI();
 ICICI icici = new ICICI();
 // Calling the interest_rate() method for each object
 System.out.println("Calling interest_rate() method for the Bank class:");
 bank.interest_rate();
 System.out.println("\nCalling interest_rate() method for the SBI class:");
 sbi.interest_rate();
 System.out.println("\nCalling interest_rate() method for the ICICI class:");
 icici.interest_rate();
 // Closing the scanner
 scanner.close();
 }
}
Output:-
Calling interest_rate() method for the Bank class:
Interest Rate in the Bank class: 4%
Calling interest_rate() method for the SBI class:
Interest Rate in SBI: 5%
Calling interest_rate() method for the ICICI class:
Interest Rate in ICICI: 6%
Problem Statement :-
2. Write a program to declare class Shape then calculate Area of circle, Area
of Triangle, Area of Rectangle and area of Square using Constructor
overloading.
import java.util.Scanner;
class Shape {
 // Common variable for all shapes
 private double area;
 // Constructor for Circle
 public Shape(double radius) {
 area = calculateCircleArea(radius);
 }
 // Constructor for Triangle
 public Shape(double base, double height) {
 area = calculateTriangleArea(base, height);
 }
 // Constructor for Rectangle
 public Shape(double length, double width, String shapeType) {
 if (shapeType.equalsIgnoreCase("rectangle")) {
 area = calculateRectangleArea(length, width);
 } else if (shapeType.equalsIgnoreCase("square")) {
 area = calculateSquareArea(length);
 } else {
 System.out.println("Invalid shape type");
 }
 }
 // Method to calculate area of a circle
 private double calculateCircleArea(double radius) {
 return Math.PI * radius * radius;
 }
 // Method to calculate area of a triangle
 private double calculateTriangleArea(double base, double height) {
 return 0.5 * base * height;
 }
 // Method to calculate area of a rectangle
 private double calculateRectangleArea(double length, double width) {
 return length * width;
 }
 // Method to calculate area of a square
 private double calculateSquareArea(double side) {
 return side * side;
 }
 // Method to display the area
 public void displayArea() {
 System.out.println("Area: " + area);
 }
}
public class ShapeAreaCalculator {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Calculate area of a circle
 System.out.print("Enter radius of the circle: ");
 double radius = scanner.nextDouble();
 Shape circle = new Shape(radius);
 System.out.println("Area of Circle:");
 circle.displayArea();
 // Calculate area of a triangle
 System.out.print("\nEnter base of the triangle: ");
 double base = scanner.nextDouble();
 System.out.print("Enter height of the triangle: ");
 double height = scanner.nextDouble();
 Shape triangle = new Shape(base, height);
 System.out.println("\nArea of Triangle:");
 triangle.displayArea();
 // Calculate area of a rectangle or square
 System.out.print("\nEnter length of the rectangle or square: ");
 double length = scanner.nextDouble();
 System.out.print("Enter width of the rectangle or type 'square' for a square:
");
 String shapeType = scanner.next();
 Shape rectangleOrSquare = new Shape(length, length, shapeType);
 System.out.println("\nArea of " + shapeType.substring(0, 1).toUpperCase() +
shapeType.substring(1) + ":");
 rectangleOrSquare.displayArea();
 // Closing the scanner
 scanner.close();
 }
}
Output:-
Enter radius of the circle: 5
Area of Circle:
Area: 78.53981633974483
Enter base of the triangle: 4
Enter height of the triangle: 8
Area of Triangle:
Area: 16.0
Enter length of the rectangle or square: 6
Enter width of the rectangle or type 'square' for a square: square
Area of Square:
Area: 36.0
Experiment No:- 8 (Interface)
Problem Statement :-
1. Write a program to implement following inheritance. Assume suitable
methods.
import java.util.Scanner;
// Interface Sports
interface Sports {
 // Member variables
 int wt = 5;
 // Method signature
 void show();
}
// Class Student implementing the Sports interface
class Student implements Sports {
 // Member variables
 int rollNo;
 String name;
 // Parameterized constructor
 public Student(int rollNo, String name) {
 this.rollNo = rollNo;
 this.name = name;
 }
 // Method from the Sports interface
 public void show() {
 System.out.println("Weightage for Sports: " + wt);
 }
 // Display method to show details of the student
 public void displayStudentDetails() {
 System.out.println("Student Details:");
 System.out.println("Roll No: " + rollNo);
 System.out.println("Name: " + name);
 }
}
// Class Result extending Student and implementing CalPercentage interface
class Result extends Student {
 // Member variables
 int marks1;
 int marks2;
 int totalMarks;
 double percentage;
 // Parameterized constructor
 public Result(int rollNo, String name, int marks1, int marks2) {
 // Calling the constructor of the superclass (Student)
 super(rollNo, name);
 this.marks1 = marks1;
 this.marks2 = marks2;
 this.totalMarks = marks1 + marks2;
 this.percentage = calculatePercentage();
 }
 // Method to calculate percentage
 private double calculatePercentage() {
 return (double) totalMarks / 2; // Assuming total marks out of 100
 }
 // Display method to show details of the student and result
 public void displayResultDetails() {
 // Calling the display method of the superclass (Student)
 displayStudentDetails();
 System.out.println("Result Details:");
 System.out.println("Marks 1: " + marks1);
 System.out.println("Marks 2: " + marks2);
 System.out.println("Total Marks: " + totalMarks);
 System.out.println("Percentage: " + percentage + "%");
 }
}
public class InheritanceAndInterfaceExample {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Accepting details for a student
 System.out.print("Enter Student Roll No: ");
 int rollNo = scanner.nextInt();
 scanner.nextLine(); // Consume the newline character
 System.out.print("Enter Student Name: ");
 String name = scanner.nextLine();
 // Accepting sports details
 System.out.print("Enter Marks 1 for Sports: ");
 int marks1 = scanner.nextInt();
 System.out.print("Enter Marks 2 for Sports: ");
 int marks2 = scanner.nextInt();
 // Creating an object of the Result class
 Result studentResult = new Result(rollNo, name, marks1, marks2);
 // Displaying details using the method of the Result class
 studentResult.displayResultDetails();
 // Calling the show() method from the Sports interface
 studentResult.show();
 // Closing the scanner
 scanner.close();
 }
}
Output:-
Enter Student Roll No: 101
Enter Student Name: John Doe
Enter Marks 1 for Sports: 8
Enter Marks 2 for Sports: 7
Student Details:
Roll No: 101
Name: John Doe
Result Details:
Marks 1: 8
Marks 2: 7
Total Marks: 15
Percentage: 7.5%
Weightage for Sports: 5
Problem Statement :-
2. Write a program to implement following inheritance. Assume suitable
methods.
import java.util.Scanner;
// Interface Employee
interface Employee {
 // Member variables
 double B_salary = 0; // Basic Salary
 double HRA = 0; // House Rent Allowance
 double DA = 0; // Dearness Allowance
 // Method signature
 void show();
}
// Class Student
class Student {
 // Member variables
 int rollNo;
 String name;
 // Method to input details
 public void input() {
 Scanner scanner = new Scanner(System.in);
 System.out.print("Enter Roll No: ");
 rollNo = scanner.nextInt();
 scanner.nextLine(); // Consume the newline character
 System.out.print("Enter Name: ");
 name = scanner.nextLine();
 scanner.close();
 }
 // Method to output details
 public void output() {
 System.out.println("Student Details:");
 System.out.println("Roll No: " + rollNo);
 System.out.println("Name: " + name);
 }
}
// Class Manager extending Student and implementing Employee interface
class Manager extends Student implements Employee {
 // Member variables
 int M_id;
 double Total_Sal;
 // Method to calculate total salary
 public void CalcSalary() {
 Total_Sal = B_salary + HRA + DA;
 }
 // Method to display details
 public void displayManagerDetails() {
 // Calling the output method of the superclass (Student)
 output();
 System.out.println("Manager Details:");
 System.out.println("Manager ID: " + M_id);
 System.out.println("Total Salary: " + Total_Sal);
 }
 // Implementation of the show method from the Employee interface
 public void show() {
 System.out.println("Employee Details:");
 System.out.println("Basic Salary: " + B_salary);
 System.out.println("House Rent Allowance: " + HRA);
 System.out.println("Dearness Allowance: " + DA);
 }
}
public class InheritanceAndInterfaceExample {
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 // Creating an object of the Manager class
 Manager manager = new Manager();
 // Input details for the manager
 System.out.println("Enter Manager Details:");
 manager.input();
 // Input additional details for the manager
 System.out.print("Enter Manager ID: ");
 manager.M_id = scanner.nextInt();
 // Calculate total salary for the manager
 manager.CalcSalary();
 // Displaying details using the method of the Manager class
 manager.displayManagerDetails();
 // Calling the show() method from the Employee interface
 manager.show();
 // Closing the scanner
 scanner.close();
 }
}
Output:-
Enter Manager Details:
Enter Roll No: 101
Enter Name: John Doe
Enter Manager ID: 001
Student Details:
Roll No: 101
Name: John Doe
Manager Details:
Manager ID: 001
Total Salary: 0.0
Employee Details:
Basic Salary: 0.0
House Rent Allowance: 0.0
Dearness Allowance: 0.0
Experiment No: - 9 (Exception Handling)
Problem Statement :-
1. Write a program to create own exception (user defined exception) to
accept no. from user and throw an exception if the number is not even.
import java.util.Scanner;
// Custom exception class
class NotEvenNumberException extends Exception {
 public NotEvenNumberException(String message) {
 super(message);
 }
}
public class CustomExceptionExample {
 // Method to accept a number and throw an exception if it's not even
 public static void checkEvenNumber(int number) throws
NotEvenNumberException {
 if (number % 2 != 0) {
 throw new NotEvenNumberException("Error: Not an even number.");
 }
 }
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 try {
 // Accepting a number from the user
 System.out.print("Enter an even number: ");
 int userInput = scanner.nextInt();
 // Checking if the number is even
 checkEvenNumber(userInput);
 // If the number is even, display a success message
 System.out.println("Entered number is even.");
 } catch (NotEvenNumberException e) {
 // Catching the custom exception and displaying the error message
 System.out.println(e.getMessage());
 } catch (Exception e) {
 // Catching other exceptions (e.g., InputMismatchException)
 System.out.println("Error: Invalid input. Please enter an integer.");
 } finally {
 // Closing the scanner
 scanner.close();
 }
 }
}
Output:-
Enter an even number: 7
Error: Not an even number.
Enter an even number: 12
Entered number is even.
Problem Statement :-
2. Write a program to create own exception (user defined exception) to
accept no. from user and throw an exception if the number is not Prime.
import java.util.Scanner;
// Custom exception class
class NotPrimeNumberException extends Exception {
 public NotPrimeNumberException(String message) {
 super(message);
 }
}
public class CustomExceptionExample {
 // Method to check if a number is prime
 public static boolean isPrime(int number) {
 if (number <= 1) {
 return false;
 }
 for (int i = 2; i <= Math.sqrt(number); i++) {
 if (number % i == 0) {
 return false;
 }
 }
 return true;
 }
 // Method to accept a number and throw an exception if it's not prime
 public static void checkPrimeNumber(int number) throws
NotPrimeNumberException {
 if (!isPrime(number)) {
 throw new NotPrimeNumberException("Error: Not a prime number.");
 }
 }
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 try {
 // Accepting a number from the user
 System.out.print("Enter a prime number: ");
 int userInput = scanner.nextInt();
 // Checking if the number is prime
 checkPrimeNumber(userInput);
 // If the number is prime, display a success message
 System.out.println("Entered number is prime.");
 } catch (NotPrimeNumberException e) {
 // Catching the custom exception and displaying the error message
 System.out.println(e.getMessage());
 } catch (Exception e) {
 // Catching other exceptions (e.g., InputMismatchException)
 System.out.println("Error: Invalid input. Please enter an integer.");
 } finally {
 // Closing the scanner
 scanner.close();
 }
 }
}
Output:-
Enter a prime number: 12
Error: Not a prime number.
Enter a prime number: 7
Entered number is prime.
Problem Statement :-
3. Write a program to create own exception (user defined exception) to accept
age from user and throw an exception if the age is negative.
import java.util.Scanner;
// Custom exception class
class NegativeAgeException extends Exception {
 public NegativeAgeException(String message) {
 super(message);
 }
}
public class CustomExceptionExample {
 // Method to accept age and throw an exception if it's negative
 public static void checkAge(int age) throws NegativeAgeException {
 if (age < 0) {
 throw new NegativeAgeException("Error: Age cannot be negative.");
 }
 }
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 try {
 // Accepting age from the user
 System.out.print("Enter your age: ");
 int userAge = scanner.nextInt();
 // Checking if the age is negative
 checkAge(userAge);
 // If the age is non-negative, display a success message
 System.out.println("Entered age is: " + userAge);
 } catch (NegativeAgeException e) {
 // Catching the custom exception and displaying the error message
 System.out.println(e.getMessage());
 } catch (Exception e) {
 // Catching other exceptions (e.g., InputMismatchException)
 System.out.println("Error: Invalid input. Please enter a valid age.");
 } finally {
 // Closing the scanner
 scanner.close();
 }
 }
}
Output:-
Enter your age: 25
Entered age is: 25
Enter your age: -5
Error: Age cannot be negative.
Problem Statement :-
4. Write a program to create own exception (user defined exception) to accept
String from user and throw an exception if the string is not starting character ‘s’.
import java.util.Scanner;
// Custom exception class
class NotStartsWithSException extends Exception {
 public NotStartsWithSException(String message) {
 super(message);
 }
}
public class CustomExceptionExample {
 // Method to accept a string and throw an exception if it doesn't start with 's'
 public static void checkStartsWithS(String input) throws
NotStartsWithSException {
 if (!input.toLowerCase().startsWith("s")) {
 throw new NotStartsWithSException("Error: String must start with 's'.");
 }
 }
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 try {
 // Accepting a string from the user
 System.out.print("Enter a string starting with 's': ");
 String userInput = scanner.nextLine();
 // Checking if the string starts with 's'
 checkStartsWithS(userInput);
 // If the string starts with 's', display a success message
 System.out.println("Entered string is: " + userInput);
 } catch (NotStartsWithSException e) {
 // Catching the custom exception and displaying the error message
 System.out.println(e.getMessage());
 } catch (Exception e) {
 // Catching other exceptions
 System.out.println("Error: Invalid input. Please enter a valid string.");
 } finally {
 // Closing the scanner
 scanner.close();
 }
 }
}
Output:-
Enter a string starting with 's': Summer
Entered string is: Summer
Enter a string starting with 's': Rainy
Error: String must start with 's'.
Problem Statement :-
5. Write a program to create own exception (user defined exception) to accept
Password from user and throw an “AuthenticationFailure” exception if the
password is incorrect.
import java.util.Scanner;
// Custom exception class
class AuthenticationFailureException extends Exception {
 public AuthenticationFailureException(String message) {
 super(message);
 }
}
public class CustomExceptionExample {
 // Method to authenticate the password and throw an exception if it's incorrect
 public static void authenticatePassword(String password) throws
AuthenticationFailureException {
 // Here, you can define your own conditions for a valid password
 // For simplicity, let's assume a valid password is "securepassword"
 if (!password.equals("securepassword")) {
 throw new AuthenticationFailureException("Error: Authentication failure.
Incorrect password.");
 }
 }
 public static void main(String[] args) {
 Scanner scanner = new Scanner(System.in);
 try {
 // Accepting a password from the user
 System.out.print("Enter your password: ");
 String userPassword = scanner.nextLine();
 // Authenticating the password
 authenticatePassword(userPassword);
 // If the password is correct, display a success message
 System.out.println("Authentication successful.");
 } catch (AuthenticationFailureException e) {
 // Catching the custom exception and displaying the error message
 System.out.println(e.getMessage());
 } catch (Exception e) {
 // Catching other exceptions
 System.out.println("Error: Invalid input. Please enter a valid password.");
 } finally {
 // Closing the scanner
 scanner.close();
 }
 }
}
Output:-
Enter your password: securepassword
Authentication successful.
Enter your password: incorrectpassword
Error: Authentication failure. Incorrect password.
Experiment No: - 10 (Package)
• java.lang: This package contains fundamental classes that are automatically
imported into every Java program. It includes classes like String, Object, and basic
data types.
• java.util: This package contains utility classes and data structures like lists, sets,
maps, and more. It includes the ArrayList, HashMap, LinkedList, etc.
• java.io: This package provides classes for input and output operations. It includes
classes for reading and writing files, working with streams, and handling
serialization.
• java.net: This package contains classes for networking, including sockets, URLs,
and network protocols. It's used for developing network applications.
• java.awt: This package provides classes for creating graphical user interfaces (GUI).
It includes components like buttons, frames, and layout managers.
• javax.swing: Building on java.awt, this package provides additional GUI
components and features. It includes components like JFrame, JButton, and more.
• java.sql: This package provides classes and interfaces for database connectivity.
It's used for interacting with relational databases using Java Database Connectivity
(JDBC).
• java.text: This package provides classes for formatting and parsing text, dates, and
numbers. It includes classes like SimpleDateFormat and DecimalFormat.
• java.time: Introduced in Java 8, this package contains classes for handling dates
and times in a more comprehensive and flexible way compared to the older
java.util.Date and java.util.Calendar classes.
• java.nio: This package provides support for non-blocking I/O operations and
improved file system handling. It includes classes like Path, Files, and Channels.
Experiment No: - 11
Problem Statement :-
Write a javascript program on client side scripting.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Client-Side Scripting with JavaScript</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 text-align: center;
 margin: 50px;
 }
 </style>
</head>
<body>
 <h1>Client-Side Scripting with JavaScript</h1>
 <button id="clickButton">Click Me!</button>
 <script>
 // JavaScript code for client-side scripting
 // Function to be executed when the button is clicked
 function handleClick() {
 // Display an alert
 alert('Button Clicked!');
 }
 // Get the button element by its ID
 var button = document.getElementById('clickButton');
 // Attach the handleClick function to the button's click event
 button.addEventListener('click', handleClick);
 </script>
</body>
</html>
Experiment No: - 12
Problem Statement :-
Write a JavaScript program on User Defined Function.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>User Defined Function in JavaScript</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 text-align: center;
 margin: 50px;
 }
 </style>
</head>
<body>
 <h1>User Defined Function in JavaScript</h1>
 <label for="lengthInput">Enter Length of Rectangle:</label>
 <input type="number" id="lengthInput" placeholder="Length">
 <label for="widthInput">Enter Width of Rectangle:</label>
 <input type="number" id="widthInput" placeholder="Width">
 <button onclick="calculateArea()">Calculate Area</button>
 <p id="resultArea"></p>
 <script>
 // JavaScript code with user-defined functions
 // Function to calculate the area of a rectangle
 function calculateRectangleArea(length, width) {
 return length * width;
 }
 // Function to be executed when the button is clicked
 function calculateArea() {
 // Get user input values
 var length = parseFloat(document.getElementById('lengthInput').value);
 var width = parseFloat(document.getElementById('widthInput').value);
 // Check if the input is valid
 if (isNaN(length) || isNaN(width)) {
 alert('Please enter valid numeric values for length and width.');
 return;
 }
 // Call the user-defined function to calculate the area
 var area = calculateRectangleArea(length, width);
 // Display the result
 document.getElementById('resultArea').textContent = 'Area of the
rectangle: ' + area;
 }
 </script>
</body>
</html>
Experiment No: - 13
Problem Statement :-
Write a JavaScript program on validation using object function.
<!DOCTYPE html>
<html lang="en">
<head>
 <meta charset="UTF-8">
 <meta name="viewport" content="width=device-width, initial-scale=1.0">
 <title>Form Validation using Object and Functions</title>
 <style>
 body {
 font-family: Arial, sans-serif;
 text-align: center;
 margin: 50px;
 }
 .error {
 color: red;
 }
 </style>
</head>
<body>
 <h1>Form Validation using Object and Functions</h1>
 <form id="registrationForm" onsubmit="validateForm(); return false;">
 <label for="name">Name:</label>
 <input type="text" id="name" placeholder="Enter your name">
 <br>
 <label for="email">Email:</label>
 <input type="email" id="email" placeholder="Enter your email">
 <br>
 <label for="password">Password:</label>
 <input type="password" id="password" placeholder="Enter your password">
 <br>
 <button type="submit">Submit</button>
 </form>
 <div id="errorMessages" class="error"></div>
 <script>
 // JavaScript code for validation using object and functions
 // Object to hold validation functions
 var validator = {
 validateName: function(name) {
 return /^[a-zA-Z\s]+$/.test(name);
 },
 validateEmail: function(email) {
 // Basic email validation for demonstration purposes
 return /^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email);
 },
 validatePassword: function(password) {
 // Basic password validation for demonstration purposes
 return password.length >= 6;
 }
 };
 // Function to validate the form
 function validateForm() {
 // Get form input values
 var name = document.getElementById('name').value.trim();
 var email = document.getElementById('email').value.trim();
 var password = document.getElementById('password').value;
 // Clear previous error messages
 document.getElementById('errorMessages').textContent = '';
 // Validate name
 if (!validator.validateName(name)) {
 document.getElementById('errorMessages').textContent += 'Invalid
name. ';
 }
 // Validate email
 if (!validator.validateEmail(email)) {
 document.getElementById('errorMessages').textContent += 'Invalid
email. ';
 }
 // Validate password
 if (!validator.validatePassword(password)) {
 document.getElementById('errorMessages').textContent += 'Invalid
password (should be at least 6 characters). ';
 }
 // Display success message if no errors
 if (document.getElementById('errorMessages').textContent === '') {
 alert('Form submitted successfully!');
 }
 }
 </script>
</body>
</html>
