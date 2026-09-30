# Arrays and Methods

## Exercises

## 05-0: Student Average

In **IntelliJ IDEA**, create a **New Project** called **StudentAverageMethod**.

In the **src** folder create a **Java class** file called *StudentAverageMethod.java* with the following source code.

Modify the starter code below so that the `average` method returns the average of an array of integers as a **double** value.

```java
import java.util.Arrays;  
  
public class StudentAverageMethod {  
    public static void main(String[] args) {  
  
            int[] marks = {75, 82, 90, 95, 87, 80, 70, 92};  
  
            System.out.printf("Marks: %s\n", Arrays.toString(marks));  
            System.out.printf("Average:  %.2f", average(marks) );  
  
  
    }  
  
    public static double average(int[] m) {  
        return 0.0;  
    }  
}
```

## 05-1: Minimum

In **IntelliJ IDEA**, create a **New Project** called **MinimumArrayMethod**.

In the **src** folder create a **Java class** file called *MinimumArrayMethod.java* with the following source code.

Modify the starter code below so that the `minimum` method returns the smallest value in an array of integers.

```java
import java.util.Arrays;  
  
public class MinimumArrayMethod {  
    public static void main(String[] args){  
            int[] marks = {75, 82, 90, 95, 87, 80, 70, 92};  
  
            System.out.printf("%s\n", Arrays.toString(marks));  
            System.out.printf("Minimum:  %d", minimum(marks));  
    }  
  
    public static int minimum(int[] m) {  
        return 0;  
    }  
}
```

## 05-2: Sum

In **IntelliJ IDEA**, create a **New Project** called **SumArrayMethod**.

In the **src** folder create a **Java class** file called *SumArrayMethod.java* with the following source code.

Modify the starter code below so that the `sum` method returns the sum of the values in an array of integers.

```java
import java.util.Arrays;  
  
public class SumArrayMethod {  
    public static void main(String[] args){  
        int[] marks = {75, 82, 90, 95, 87, 80, 70, 92};  
  
        System.out.printf("%s\n", Arrays.toString(marks));  
        System.out.printf("Sum:  %d", sum(marks));  
    }  
  
    public static int sum(int[] m) {  
        return 0;  
    }  
}
```

## 05-3: Randomize

In **IntelliJ IDEA**, create a **New Project** called **RandomizeMethod**.

In the **src** folder create a **Java class** file called *RandomizeMethod.java*.

Complete the definition of the method `randomize` whose header is

```java
public static int[] randomize(int n)
```

The method should return an array of size `n` whose elements are the values `0...n-1` *(inclusive)* ordered randomly. As an example, `randomize(5)` might return `[4, 2, 0, 3, 1]`. Include an example using the `randomize` method in your `main` method.

## 05-4: Polynomial

In **IntelliJ IDEA**, create a **New Project** called **Polynomial**.

In the **src** folder create a **Java class** file called *Polynomial.java*.

A *polynomial* in `x` of degree `n` is an expression of the form

$$
a_nx^n + a_{n-1}x^{n-1} +...+ a_2 x^2 + a_1x + a_0
$$
where $a_n \neq 0$.

The values $a_0, a_1, ..., a_n$ are called the *coefficients* of the polynomial. Complete the definition of the method `eval` so that it returns the value at `x` of a polynomial whose coefficients are stored in the array `a`.

```java
public static double eval(double[] a, double x)
```

As an example, `randomize([1,-2, -8], 3)` would return `7`, since it represents the value of $f(3)$, where

$$
f(x) = x^2 -2x -8
$$
Include two examples using the `eval` method in your `main` method.

## 05-5: Tic-Tac-Toe Exercises

These exercises demonstrate how you might use a single-dimensional array in Java to store information in a grid-based game like Tic-Tac-Toe . In this case a 9 element array is used to store the 9 possible positions of the tic-tac-toe game. The index values of the array  match the grid positions given in the table below.

|   Tic  |  Tac   |  Toe   |
|:---:|:---:|:---:|
|  0  |  1  |  2  |
|  3  |  4  |  5  |
|  6  |  7  |  8  |


## Board Setup

The **board** array is filled initially with the values ```X```, ```O```, or ```-```.  In this game, this value will represent an empty square and be displayed as ```-```.  See the starter code below.

## Tasks

In **IntelliJ IDEA**, create a **New Project** called **TicTacToe**.

In the **src** folder create a **Java class** file called *TicTacToe.java* with the following source code.

```java
public class TicTacToe {  
    public static void main(String[] args) {  
	    char[] board = {'X', 'O', 'X', 'O', 'X', '-', '-', 'X', 'O'};  
	    display(board);
	    System.out.println();  
	    System.out.println("Win? " + isWin(board));  
	    System.out.println("Tie? " + isTie(board));
    }  
  
    public static void display(char[] b) {  
        for (int i=0; i < b.length; i++) {  
            if (i % 3 == 0) {  
                System.out.printf("\n%c  ", b[i]);  
            } else {  
                System.out.printf("%c  ", b[i]);  
            }  
        }    
    }  
  
    public static boolean isWin(char[] b) {  
        return false;  
    }  
  
    public static boolean isTie(char[] b) {  
        return false;  
    }  
}
```

## 05-3-1:  Is there a Win?

Complete the **isWin()** function. It should return **true** if there is a win on the board.  Otherwise, it should return **false**. Remember, there are 8 possible ways to win in the tic-tac-toe game:  3 of the same kind _('X' or 'O')_ in any row _(3)_, any column _(3)_, or either diagonal _(2)_.

## 05-3-2:  Is there a Tie?
Complete the **isTie()** function. It should return **true** if there is a tie on the board.  Otherwise, it should return **false**.  A **tie** occurs if the board is filled, with 'X's and 'O's but there is **no win**.
