# GravityCalculator
Create a program that computes the distance an object will fall in Earth's gravity. 

Original Code:
```Java
class GravityCalculator {
    public static void main(String[] arguments) {
        double gravity = -9.81; // Earth's gravity in m/s^2
        double initialVelocity = 0.0;
        double fallingTime = 10.0;
        double initialPosition = 0.0;
        double finalPosition = 0.0;
        System.out.println("The object's position after " + fallingTime + " seconds is " + finalPosition + " m.");
    }
}
```
output:

![output(1)](https://user-images.githubusercontent.com/85108203/154523779-e49641e1-a5f3-4cd4-abf0-6f7a4fc35bb0.png)

Modify the example program to compute the position of an object after falling for 10 seconds, outputting the position in meters. The formula in Math notation is: x(t) = 0.5 × at 2 + vit + xi Variable Meaning Value a Acceleration (m/s 2 ) -9.81 t Time (s) 10 vi Initial velocity (m/s) 0 xi Initial position 0 Note: The correct value is -490.5 m. Java will output more digits after the decimal place, but that is unimportant.

Modified Code:

```Java
 class GravityCalculator {
        public static void main(String[] arguments) {
            double gravity = -9.81; // Earth's gravity in m/s^2
            double initialVelocity = 0.0;
            double fallingTime = 10.0;
            double initialPosition = 0.0;
            double finalPosition = 0.0;
            double x; /*finalPosition = 0.0;*/
            x=(0.5 * ( gravity * (fallingTime * fallingTime)) + (initialVelocity * fallingTime) + (initialPosition));
            System.out.println("The object's position after " + fallingTime + " seconds is " + x /*finalPosition + */  + " m.");        }
    }
```

Output:

![output(2)](https://user-images.githubusercontent.com/85108203/154524240-870f3e9e-4bf4-49fd-bdfe-9ed6b8dc7ed4.png)
