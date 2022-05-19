# Recursion Algorithms

* In Java, a method that calls itself is known as a recursive method. And, this process is known as recursion.

* A physical world example would be to place two parallel mirrors facing each other. Any object in between them would be reflected recursively.
  
 #### How Recursion works?
  
  ![image](https://user-images.githubusercontent.com/40323661/168844437-5989bb52-f1ae-4cf0-839d-ec9c1b3233ac.png)

* In the above example, we have called the recurse() method from inside the main method. (normal method call). And, inside the recurse() method, we are again calling the same recurse method. This is a recursive call.

* In order to stop the recursive call, we need to provide some conditions inside the method. Otherwise, the method will be called infinitely.

* Hence, we use the if...else statement (or similar approach) to terminate the recursive call inside the method.
  
 #### Example: Factorial of a Number Using Recursion
 
 ```Java
   class Factorial {

    static int factorial( int n ) {
        if (n != 0)  // termination condition
            return n * factorial(n-1); // recursive call
        else
            return 1;
    }

    public static void main(String[] args) {
        int number = 4, result;
        result = factorial(number);
        System.out.println(number + " factorial = " + result);
    }
}

  OR
  
  
   static int factorial( int n ) {
        if (n == 1)  // termination condition
            return 1; //
        else
            return n * factorial(n-1);  recursive call
    }

    public static void main(String[] args) {
        int number = 4, result;
        result = factorial(number);
        System.out.println(number + " factorial = " + result);
    }
  
  
 ```
 
![image](https://user-images.githubusercontent.com/40323661/168845604-608e9a56-4094-4b61-b6c9-9306decd97a4.png)

#### Advantages and Disadvantages of Recursion

* When a recursive call is made, new storage locations for variables are allocated on the stack. As, each recursive call returns, the old variables and parameters are removed from the stack. Hence, recursion generally uses more memory and is generally slow.

* On the other hand, a recursive solution is much simpler and takes less time to write, debug and maintain.
  
![image](https://user-images.githubusercontent.com/40323661/168847911-e863c2ae-cb8c-46a9-ba13-39d203360c5e.png)
   
#### The program to implement the Fibonacci series is given below:

```Java
public class Fibonacci1 {

	    //method to calculate fibonacci series
	    static int fibonacci(int n) {
	        if (n <= 1) {
	            return n;
	        }
	        return fibonacci(n-1) + fibonacci(n-2);
	    }
	    public static void main(String[] args) {
	        int number = 10;
	  
	        //print first 10 numbers of fibonacci series
	        System.out.println ("Fibonacci Series: First 10 numbers:");
	        for (int i = 1; i <= number; i++) 
	        {
	            System.out.print(fibonacci(i) + " ");
	        }
	  
	}
	}
```
#### Reverse String Recursion Java

* Given a string “Hello” we have to reverse it so that the resultant string is “olleH”.

* This is done using recursion. Starting from the last character in the string we recursively print each character until all the characters in the string are exhausted.

```Java

package com.veer.algo.recursion;

public class String_Reverse {

	public static void main(String[] args) {
		String inputstr = "SoftwareTestingHelp";
		System.out.println("The given string: " + inputstr);
		String_Reverse obj = new String_Reverse();
		System.out.print("The reversed string: ");
		obj.reverseString(inputstr);

	}

	// recursive method to reverse a given string
	void reverseString(String str) {
		// base condition; return if string is null or with 1 or less character
		if ((str == null) || (str.length() <= 1))
			System.out.println(str);
		else {
			// recursively print each character in the string from the end
			System.out.print(str.charAt(str.length() - 1));
			reverseString(str.substring(0, str.length() - 1));
		}
	}
}

```
![image](https://user-images.githubusercontent.com/40323661/169180783-9bc2404f-19ff-4f8f-a998-ce9808187c18.png)


