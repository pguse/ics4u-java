
# Designing Classes in Java - Introduction

In **IntelliJ IDEA**, create a **New Project** called **Cartesian**.

In the **src** folder create a **Java class** file called *Cartesian.java* with the following source code.

## Exercises

Complete the following exercises by creating methods in a **Point** class contained in a Java class file called *Point.java*.

```java
public class Point {  
    private int x;  
    private int y;  
  
    public Point(int x, int y) {  
        this.x = x;  
        this.y = y;  
    }  
  
    public int getX() {  
        return x;  
    }  
  
    public int getY() {  
            return y;  
    }  
  
    @Override  
    public String toString() {  
        return "( " + this.x + ", " + this.y + ")";  
    }  
}
```
## 06-0:  Distance

Complete the following function, that returns the **distance between two points**. Implement the `distance` method on an instance of type `Point` in the ```main``` method of a ```Main.java``` file.

```java
public double distance(Point p) {
	return 0.0;
}
```

## 06-1:  Slope

Complete the following function, that returns the **slope of a line passing through two points**. Implement the `slope` method on an instance of type `Point` in the ```main``` method of a ```Main.java``` file.

```java
public double slope(Point p) {
	return 0.0;
}
```

In **IntelliJ IDEA**, create a **New Project** called Fraction.

In the **src** folder create a **Java class** file called *Fraction.java* with the following source code.
Complete the following exercises by creating methods in a **Fraction** class contained in a Java class file called *Fraction.java*.

## 06-2:  Multiply

Complete the following method, that returns the **product** of an **instance** of **Fraction** and another **Fraction** f. Implement the `mult` method on an instance of type `Fraction` in the ```main``` method of a ```Main.java``` file.

```java
public Fraction mult(Fraction f) {
	return new Fraction(1,1);
}
```

## 06-3:  Divide

Complete the following method, that returns the **quotient** of an **instance** of **Fraction** and another **Fraction** f. Implement the `div` method on an instance of type `Fraction` in the ```main``` method of a ```Main.java``` file.

```java
public Fraction div(Fraction f) {
	return new Fraction(1,1);
}
```

## 06-4:  Add

Complete the following method, that returns the **sum** of an **instance** of **Fraction** and another **Fraction** f. Implement the `add` method on an instance of type `Fraction` in the ```main``` method of a ```Main.java``` file.

```java
public Fraction add(Fraction f)  {
	return new Fraction(1,1);
}
```

## 06-5:  Subtract

Complete the following method, that returns the **difference** of an **instance** of **Fraction** and another **Fraction** f. Implement the `subt` method on an instance of type `Fraction` in the ```main``` method of a ```Main.java``` file.

```java
public Fraction subt(Fraction f) {
	return new Fraction(1,1);
}
```
