# Experiment 1a

## AIM : display primitive data types

``` java
class exp_1a{
byte b;
short s;
int i;
long l;
double d;
float f;
char c;
boolean bool;
public static void main(String arg[]){
exp_1a obj = new exp_1a();
System.out.println("default primitive datatypes:");
System.out.println("default byte:"+obj.b);
System.out.println("short:"+obj.s);
System.out.println("int:"+obj.i);
System.out.println("long:"+obj.l);
System.out.println("double:"+obj.d);
System.out.println("float:"+obj.f);
System.out.println("char:"+obj.c+"");
System.out.println("bool:"+obj.bool);
}}
```

## output:

![the default values of all the DataTypes](1aoutput.png)


# experiment 1b
## AIM: find the roots of quadratic equation and nature of the roots
``` java
import java.util.Scanner;

 class QuadraticEquation {
    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter coefficient a: ");
        double a = sc.nextDouble();

        System.out.print("Enter coefficient b: ");
        double b = sc.nextDouble();

        System.out.print("Enter coefficient c: ");
        double c = sc.nextDouble();

        double discriminant = b * b - 4 * a * c;

        if (discriminant > 0) {
            System.out.println("Roots are real and distinct.");

            double root1 = (-b + Math.sqrt(discriminant)) / (2 * a);
            double root2 = (-b - Math.sqrt(discriminant)) / (2 * a);

            System.out.println("Root 1: " + root1);
            System.out.println("Root 2: " + root2);

        } else if (discriminant == 0) {
            System.out.println("Roots are real and equal.");

            double root = -b / (2 * a);
            System.out.println("Root: " + root);

   } else {
            System.out.println("Roots are complex and imaginary.");

            double realPart = -b / (2 * a);
            double imaginaryPart = Math.sqrt(-discriminant) / (2 * a);

            System.out.println("Root 1: " + realPart + " + " + imaginaryPart + "i");
            System.out.println("Root 2: " + realPart + " - " + imaginaryPart + "i");
        }

        sc.close();
    }
}

```
## output:
![Nature of all the root types](exp_1boutput.png)
