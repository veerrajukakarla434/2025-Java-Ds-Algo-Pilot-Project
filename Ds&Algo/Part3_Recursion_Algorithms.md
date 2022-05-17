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
 ```
 
![image](https://user-images.githubusercontent.com/40323661/168845604-608e9a56-4094-4b61-b6c9-9306decd97a4.png)

#### Advantages and Disadvantages of Recursion

* When a recursive call is made, new storage locations for variables are allocated on the stack. As, each recursive call returns, the old variables and parameters are removed from the stack. Hence, recursion generally uses more memory and is generally slow.

* On the other hand, a recursive solution is much simpler and takes less time to write, debug and maintain.
  
