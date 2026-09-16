# Working with Numbers

## Exercises

## 01-0: Student Average

In **IntelliJ IDEA**, create a **New Project** called **StudentAverage**.

In the **src** folder create a **Java class** file called *StudentAverage.java* with the following source code

```java
public class StudentAverage {  
    public static void main(String[] args) {  
        int m1 = 80;  
        int m2 = 92;  
        int m3 = 88;  
  
        int average = (m1 + m2 + m3) / 3;  
        System.out.println("Average is: " + average);  
    }  
}
```

1. Click the **play** button to run the program.  Something isn't right.  Everything seems fine, but the way **Java** performs division depends on the types of the operands.  Check with your calculator.  Is the quotient of the division correct?  If not what do you think needs to be changed?
2. Make the necessary changes to produce the correct answer.
3.  Format the output average with **two decimal places** by using the **printf** method.

## 01-1: Volume of a Cylinder

In **IntelliJ IDEA**, create a **New Project** called **Volume**.

In the **src** folder create a **Java class** file called *Volume.java* with the following source code

```java
public class Volume {  
    public static void main(String[] args) {  
        double radius = 2.0;  
        double area = Math.PI * radius * radius;  
        System.out.println("Area of the circle: " + area);  
    }  
}
```

1. Modify the program to calculate the volume of a cylinder: $V = \pi r^2 h$
2. Format the output the produce an answers with 1 decimal place.
3. Modify the program to use the **Math.pow()** method to square the radius instead of using multiplication.

## 01-2: Hypotenuse of a Right-Angled Triangle

In **IntelliJ IDEA**, create a **New Project** called **Hypotenuse**.

In the **src** folder create a **Java class** file called *Hypotenuse.java* with the following source code

```java
public class Hypotenuse {  
    public static void main(String[] args) {  
        int a = 3;  
        int b = 4;  
        int sum = a + b;  
        int hypotenuse = Math.sqrt(sum);  
        System.out.println("Hypotenuse" + hypotenuse);  
    }  
}
```

1. Run the code.  Can you figure out what is wrong? There are two mistakes in the code.
2. Format the output so that it has one decimal place.

## 01-3: Swap Digits *(using the modulus % operator)*

In **IntelliJ IDEA**, create a **New Project** called **Swap**.

In the **src** folder create a **Java class** file called *Swap.java* with the following source code

```java
public class Swap {  
    public static void main(String[] args) {  
        int number = 75;  
        int swap;  
  
        System.out.println("Tens: " + number / 10);  
        System.out.println("Remainder: " + number % 10);  
    }  
}
```

1. Modify the starter code so that it swaps the digits of the variable *number*. You should **save** the new value in a variable called *swap* and output its value use the method **println()**.  *Assume that the number you are swapping only has two digits.*  **Note:** The */* operator returns the **quotient** of a division of two integers, while the **modulus** operator *%* returns the **remainder** of a division of two integers.

## 01-4: Three-Digit Number

In **IntelliJ IDEA**, create a **New Project** called **Digits**.

In the **src** folder create a **Java class** file called *Digits.java*.

Write a program that:

1. Stores a three-digit number
2. Finds the sum of the digits of the number
3. Prints **both** the number and its digit sum

## 01-5: Escape Velocity

In **IntelliJ IDEA**, create a **New Project** called **EscapeVelocity**.

In the **src** folder create a **Java class** file called *EscapeVelocity.java*.

In order for an object to escape a planet's gravitational pull, it must attain a minimum initial velocity called the *escape velocity*. The escape velocity varies from planet to planet but it is the same for all objects on the planet. Assume that we are analyzing the data that a small probe has collected while exploring some mystery planet. The probe has managed to obtain the circumference of the planet and the acceleration due to gravity at the surface. The probe must now determine what initial velocity it requires for takeoff in order to remove itself from the planet's gravitational force.

You are to create a *Java* program that will determine this velocity. Your program should store the **circumference** of the planet and also the **acceleration due to gravity** on the planet. From this information your program should determine the **radius**, **mass**, and **escape velocity** of the planet using the following equations:

$v_{escape} = \sqrt{2Gm \over r}$

and

$a = {Gm \over r^2}$

In these equations, **m** *kg* is the planet's mass, **r** *km* is the planet's radius, **G** is the gravitational constant approximated by $$6.6726 \times 10^{-11} m^3 kg^{-1} s^{-2}$$ , and **a**  $m/s^2$ is the acceleration due to gravity on the surface of the planet.

Your program should have **output** as shown in the following example:
```
Circumference (km) of planet: 38000
Acceleration due to gravity (m/s^2) on planet: 9.8

Calculating escape velocity ...
Planet radius: 6047.9 km
Planet mass: 5372.0 x 10^-21 kg
Escape velocity: 10.9 km/s
```
**Note:**  All results are *rounded* to *one decimal place* for printing. Your program must handle the unit conversions as well as printing the planet's mass in terms of $10^{21}$ kg. Assume that this will always produce reasonable results. Assume the planet is perfectly spherical.