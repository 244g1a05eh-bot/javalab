# experiment 2A
## AIM: Implementing class mechanism in java. create class. methods and invoke them inside the main method.

```java
class MyClass {

    void displayMessage() {
        System.out.println("Welcome to Java");
    }

    int add(int a, int b) {
        return a + b;
    }

    public static void main(String[] args) {

        MyClass obj = new MyClass();

        obj.displayMessage();

        int result = obj.add(10, 20);
        System.out.println("Sum: " + result);
    }
}
```
## output
![The output of 2a is](2aoutput.png)

# experiment 2b
## AIM: To implement method overloading 
```java
class OverloadExample {

    int add(int a, int b) {
        return a + b;
    }

    double add(double a, double b) {
        return a + b;
    }

    int add(int a, int b, int c) {
        return a + b + c;
    }

    public static void main(String[] args) {

        OverloadExample obj = new OverloadExample();

        System.out.println("Result of adding two integers: " + obj.add(10, 20));
        System.out.println("Result of adding two double values: " + obj.add(5.5, 4.5));
        System.out.println("Result of adding three integers: " + obj.add(1, 2, 3));
    }
}
```
## output 
![the ouput is](2boutput.png)

# experiment 2C
## AIM: to implement constructor
``` java
class Student {

    String name;
    int age;
    int marks;

    Student(String n, int a, int m) {
        name = n;
        age = a;
        marks = m;
    }

    void display() {
        System.out.println("Name: " + name);
        System.out.println("Age: " + age);
        System.out.println("Marks: " + marks);
    }

    public static void main(String[] args) {

        Student s1 = new Student("Alice", 20, 85);
        s1.display();
    }
}
```
# output
![the output is](2coutput.png)
