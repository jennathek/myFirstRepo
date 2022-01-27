# Calculating Area of Circle


1. Class Circle


```java
private final double PI = 3.14;
    private double radius;

    public Circle() {
        radius = 0.0;
    }

    public Circle(double r) {
        radius = r;
    }

    public void setRadius(double r) {
        radius = r;
    }

    public double getRadius() {
        return radius;
    }

    public double getArea() {
        return PI * Math.pow(radius, 2);
    }
```

  First, I set the value of PI as 3.14 and made 'radius' object in datatype double. And I made constructor 'setRadius' that passes the radius value to the accessor, 'getRadius'. And then 'get Area' returns the area of the circle with the radius value that is returned from 'getRadius'.
  

***



2. Class Main

```java
    Scanner input = new Scanner(System.in);

    System.out.print("Enter the radius of a circle: ");
    double radius = input.nextDouble();

    input.close();
```
    
  By creating Scanner object for input, the users can input any radius(datatype double) after they are asked to enter the radius of a circle.
    
```java
    Circle circle1 = new Circle(radius);
    
    System.out.println("Area is " + circle1.getArea());
```
  This Circle object will pass the radius that user input into the getter(getRadius).
  And it is going to print the exact Area of the circle since the getter 'getArea' is calculated with the radius that user input. 
  

    

    

