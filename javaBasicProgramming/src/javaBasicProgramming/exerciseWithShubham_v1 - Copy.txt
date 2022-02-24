package javaBasicProgramming;
import java.util.Scanner;

public class exerciseWithShubham_v1 {
	//public static final String ANSI_RESET = "\033[0m";
	//private static final String ANSI_RED = "\033[0;31m";
	private static Scanner input = new Scanner (System.in);
	public static void main(String[] args) {
		// TODO Auto-generated method stub

		// Declaring variables
		
		boolean validation;
		String choice = "";
		
		
		do {
			validation = false;
			System.out.print("\n\n\nEnter the number of the Exercise you wish to run\n"
					+ "Exercises span from 1 to 19\nExemple:\n"
					+ "1 - To run Exercise 1\n"
					+ "Q - For Quit\n"
					+ "Pick: ");
			choice = input.next().toUpperCase();
			switch(choice) {
			
			case "1":{
				Exercise_1();
				validation = true;
				break;
			}
			case "2":{
				Exercise_2();
				validation = true;
				break;
			}
			case "3":{
				Exercise_3();
				validation = true;
				break;
			}
			case "4":{
				Exercise_4();
				validation = true;
				break;
			}
			case "5":{
				Exercise_5();
				validation = true;
				break;
			}
			case "6":{
				Exercise_6();
				validation = true;
				break;
			}
			case "7":{
				Exercise_7();
				validation = true;
				break;
			}
			case "8":{
				Exercise_8();
				validation = true;
				break;
			}
			case "9":{
				Exercise_9();
				validation = true;
				break;
			}
			case "10":{
				Exercise_10();
				validation = true;
				break;
			}
			case "11":{
				Exercise_11();
				validation = true;
				break;
			}
			case "12":{
				Exercise_12();
				validation = true;
				break;
			}
			case "13":{
				Exercise_13();
				validation = true;
				break;
			}
			case "14":{
				Exercise_14();
				validation = true;
				break;
			}
			case "15":{
				Exercise_15();
				validation = true;
				break;
			}
			case "18":{
				Exercise_18();
				validation = true;
				break;
			}
			case "19":{
				Exercise_19();
				validation = true;
				break;
			}
			
			}
			
			if(validation==false) {System.out.println(/*ANSI_RED + */"\nInvalid Input!\nTry again!\n"/* + ANSI_RESET*/);}
		}while(!choice.equals("Q"));
		
		System.out.println("\n\nThank you for playing the program and checking the exercises :)\nHave a nice day now!");
		
		
		
		
	}
	
	private static void Exercise_1 () {
		System.out.println("\n\n1. Write a Java program to print 'Hello' on screen and then print your name on a separate line.\n"
				+ "Expected Output :\r\n"
				+ "Hello\r\n"
				+ "Alexandra Abramov\n\n\rMy Output:\n");
		System.out.print("Enter your name: ");
		String name = input.next() +" " + input.next();
		System.out.println("Hello\n" + name);
	}

	private static void Exercise_2 () {
		System.out.println("\n\n2. Write a Java program to print the sum of two numbers.\r\n"
				+ "Test Data:\r\n"
				+ "74 + 36\r\n"
				+ "Expected Output :\r\n"
				+ "110\n\n\nMy Output:\n");
		
		System.out.print("Enter the first number: "); int a = input.nextInt();
		System.out.print("Enter the second number: "); int b = input.nextInt();
		System.out.println("Their sum is: " + (a+b));
	}
	
	private static void Exercise_3 () {
		System.out.println("\n\n3. Write a Java program to divide two numbers and print on the screen.\r\n"
				+ "Test Data :\r\n"
				+ "50/3\r\n"
				+ "Expected Output :\r\n"
				+ "16\n\n\nMy Output:\n");
		
		System.out.print("Enter the first number: "); int a = input.nextInt();
		System.out.print("Enter the second number: "); int b = input.nextInt();
		System.out.println("Their division is: " + (a/b));
	}
	
	private static void Exercise_4 () {
		System.out.println("\n\n4. Write a Java program to print the result of the following operations.\r\n"
				+ "Test Data:\r\n"
				+ "a. -5 + 8 * 6\r\n"
				+ "b. (55+9) % 9\r\n"
				+ "c. 20 + -3*5 / 8\r\n"
				+ "d. 5 + 15 / 3 * 2 - 8 % 3\r\n"
				+ "Expected Output :\r\n"
				+ "43\r\n"
				+ "1\r\n"
				+ "19\r\n"
				+ "13\n\n\nMy Output:\n");
		
		 System.out.println("The result of the operation '-5 + 8 * 6' is: " + (-5 + 8 * 6));
		 System.out.println("The result of the operation '(55 + 9)%9' is: " + ((55 + 9)%9));
		 System.out.println("The result of the operation '20 + -3 * 5 / 8' is: " + (20 + -3 * 5 / 8));
		 System.out.println("The result of the operation '5 + 15 / 3 * 2 - 8 % 3' is: " + (5 + 15 / 3 * 2 - 8 % 3));
	}
	
	private static void Exercise_5 () {
		System.out.println("\n\n5. Write a Java program that takes two numbers as input and display the product of two numbers.\r\n"
				+ "Test Data:\r\n"
				+ "Input first number: 25\r\n"
				+ "Input second number: 5\r\n"
				+ "Expected Output :\r\n"
				+ "25 x 5 = 125\n\n\nMy Output:\n");
		
		System.out.print("Enter the first number: "); int a = input.nextInt();
		System.out.print("Enter the second number: "); int b = input.nextInt();
		System.out.println(a + " x " + b + " = " + (a*b));
	}
	
	private static void Exercise_6 () {
		System.out.println("\n\n6. Write a Java program to print the sum (addition), multiply, subtract, divide and remainder of two numbers.\r\n"
				+ "Test Data:\r\n"
				+ "Input first number: 125\r\n"
				+ "Input second number: 24\r\n"
				+ "Expected Output :\r\n"
				+ "125 + 24 = 149\r\n"
				+ "125 - 24 = 101\r\n"
				+ "125 x 24 = 3000\r\n"
				+ "125 / 24 = 5\r\n"
				+ "125 mod 24 = 5\n\n\nMy Output:\n");
		
		System.out.print("Enter the first number: "); int a = input.nextInt();
		System.out.print("Enter the second number: "); int b = input.nextInt();
		System.out.println(a + " + " + b + " = " + (a+b));
		System.out.println(a + " - " + b + " = " + (a-b));
		System.out.println(a + " x " + b + " = " + (a*b));
		System.out.println(a + " / " + b + " = " + (a/b));
		System.out.println(a + " mod " + b + " = " + (a%b));
	}
	
	private static void Exercise_7 () {
		System.out.println("\n\n7. Write a Java program that takes a number as input and prints its multiplication table upto 10.\r\n"
				+ "Test Data:\r\n"
				+ "Input a number: 8\r\n"
				+ "Expected Output :\r\n"
				+ "8 x 1 = 8\r\n"
				+ "8 x 2 = 16\r\n"
				+ "8 x 3 = 24\r\n"
				+ "...\r\n"
				+ "8 x 10 = 80\n\n\nMy Output:\n");
		
		System.out.print("Enter the number: "); int a = input.nextInt();
		for(int i=1;i<=10;i++) {
			System.out.println(a + " x " + i + " = " + (a*i));
		}
	}
	
	private static void Exercise_8 () {
		System.out.println("\n\n8. Write a Java program to display the following pattern.\r\n"
				+ "Sample Pattern :\r\n"
				+ "\r\n"
				+ "   J    a   v     v  a                                                  \r\n"
				+ "   J   a a   v   v  a a                                                 \r\n"
				+ "J  J  aaaaa   V V  aaaaa                                                \r\n"
				+ " JJ  a     a   V  a     a\r\n"
				+ "\n\n\nMy Output:\n");
		
		System.out.println("   J    a   v     v  a\n   J   a a   v   v  a a\nJ  J  aaaaa   V V  aaaaa\n JJ  a     a   V  a     a");
	}
	
	private static void Exercise_9 () {
		System.out.println("\n\n9. Write a Java program to compute the specified expressions and print the output.\r\n"
				+ "Test Data:\r\n"
				+ "((25.5 * 3.5 - 3.5 * 3.5) / (40.5 - 4.5))\r\n"
				+ "Expected Output\r\n"
				+ "2.138888888888889\n\n\nMy Output:");
		
System.out.println(((25.5 * 3.5 - 3.5 * 3.5) / (40.5 - 4.5)));
	}
	
	private static void Exercise_10 () {
		System.out.println("\n\n10. Write a Java program to compute a specified formula.\r\n"
				+ "Specified Formula :\r\n"
				+ "4.0 * (1 - (1.0/3) + (1.0/5) - (1.0/7) + (1.0/9) - (1.0/11))\r\n"
				+ "Expected Output\r\n"
				+ "2.9760461760461765\n\n\nMy Output:");
		
		System.out.println(4.0 * (1 - (1.0/3) + (1.0/5) - (1.0/7) + (1.0/9) - (1.0/11)));
	}
	
	private static void Exercise_11 () {
		System.out.println("\n\n11. Write a Java program to print the area and perimeter of a circle.\r\n"
				+ "Test Data:\r\n"
				+ "Radius = 7.5\r\n"
				+ "Expected Output\r\n"
				+ "Perimeter is = 47.12388980384689\r\n"
				+ "Area is = 176.71458676442586\n\n\nMy Output:\n");
		
		System.out.print("Enter the radius: ");double radius = input.nextDouble();
		System.out.println("The perimeter is = " + (Math.PI * 2 * radius));
		System.out.println("The Area is = " + (Math.PI * radius * radius));
	}
	
	private static void Exercise_12 () {
		System.out.println("\n\n12. Write a Java program that takes three numbers as input to calculate and print the average of the numbers.\n");
		
		System.out.print("Enter the first number: "); int a = input.nextInt();
		System.out.print("Enter the second number: "); int b = input.nextInt();
		System.out.print("Enter the third number: "); int c = input.nextInt();
		System.out.println("The average of: " + a + "; " + b + "; " + c + " is: " + ((a+b+c)/3));
	}
	
	private static void Exercise_13 () {
		System.out.println("\n\n13. Write a Java program to print the area and perimeter of a rectangle.\r\n"
				+ "Test Data:\r\n"
				+ "Width = 5.6 Height = 8.5\r\n"
				+ "\r\n"
				+ "Expected Output\r\n"
				+ "Area is 5.6 * 8.5 = 47.60\r\n"
				+ "Perimeter is 2 * (5.6 + 8.5) = 28.20\n\n\nMy Output:\n");
		
		System.out.print("Enter the Width = "); final double width = input.nextDouble();
		System.out.print("Enter the Height= "); final double height = input.nextDouble();
		System.out.printf("The Area is %.1f * %.1f = %.2f\n",width,height,(width*height));
		System.out.printf("The Perimeter is 2 * (%.1f + %.1f) = %.2f\n",width,height,(2*(width+height)));
		
	}
	
	private static void Exercise_14 () {
		System.out.println("\n\n14. Write a Java program to print an American flag on the screen.\r\n"
				+ "Expected Output\r\n"
				+ "\r\n"
				+ "* * * * * * ==================================                          \r\n"
				+ " * * * * *  ==================================                          \r\n"
				+ "* * * * * * ==================================                          \r\n"
				+ " * * * * *  ==================================                          \r\n"
				+ "* * * * * * ==================================                          \r\n"
				+ " * * * * *  ==================================                          \r\n"
				+ "* * * * * * ==================================                          \r\n"
				+ " * * * * *  ==================================                          \r\n"
				+ "* * * * * * ==================================                          \r\n"
				+ "==============================================                          \r\n"
				+ "==============================================                          \r\n"
				+ "==============================================                          \r\n"
				+ "==============================================                          \r\n"
				+ "==============================================                          \r\n"
				+ "==============================================\n\n\nMy Output:\n");
		
		System.out.println("* * * * * * ==================================\n"
				+ " * * * * *  ==================================\n"
				+ "* * * * * * ==================================\n"
				+ " * * * * *  ==================================\n"
				+ "* * * * * * ==================================\n"
				+ " * * * * *  ==================================\n"
				+ "* * * * * * ==================================\n"
				+ " * * * * *  ==================================\n"
				+ "* * * * * * ==================================\n"
				+ "==============================================\n"
				+ "==============================================\n"
				+ "==============================================\n"
				+ "==============================================\n"
				+ "==============================================\n"
				+ "==============================================");
	}
	
	private static void Exercise_15 () {
		System.out.println("\n\n15. Write a Java program to swap two variables.\n\n\nMy Output:\n");
		
		/*
		 This Exercise is my favourite out of the 15 :( THEY WERE SOOO BORING.... 
		 but this was kinda fun
		 */
		
		System.out.print("Enter the first number: "); int a = input.nextInt();
		System.out.print("Enter the second number: "); int b = input.nextInt();
		System.out.println("\nSo a,the first number, is " + a + "\nAnd b, the second number, is " + b + "\n\nNow watch them flip");
		a+=b;
		b=a-b;
		a-=b;
		System.out.println("\nNow a, the first number, is " + a + "\nAnd b, the second number, is " + b + "\n\nThis is called a quick sort");
	}
	
	
	private static void Exercise_18() {
		System.out.print("Enter the binary number: "); String a = input.next();
		System.out.print("Enter the binary number: "); String b = input.next();
		String output="";
		for (int i=0;i<(a.length() + b.length());i++) {
			output+=(a.charAt(i).intValue()*b.charAt(i).intValue());
		}
	}
	
	/*private static void Exercise_19() {
		System.out.print("Enter the number: "); int number = input.nextInt();
		int counter = 0;
		while(number/(int)(Math.pow(2,counter))!=1) {counter++;}
		number-=(int)(Math.pow(2,counter));
		System.out.print("1");
		for (int i=counter-1;i>=0;i--) {
			if(number/(int)(Math.pow(2,i))==1) {
				System.out.print("1");
				number-=Math.pow(2,i);
			}
			else {
				System.out.print("0");
			}
		}
	} */
	
	private static void Exercise_19() {
		int dec_num, quot, i=1, j;
        int bin_num[] = new int[100];
		
        System.out.print("Input a Decimal Number : ");
        dec_num = input.nextInt();
		
        quot = dec_num;
		
        while(quot != 0)
        {
            bin_num[i++] = quot%2;
            quot = quot/2;
        }
		
        System.out.print("Binary number is: ");
        for(j=i-1; j>0; j--)
        {
            System.out.print(bin_num[j]);
        }
        System.out.print("\n");
        }
	
	}
	

