---
layout: page
title: Notes
permalink: /notes/
---

### Capture Information Plan:

This is where I will store most of my general notes. If there is specific information either college board or PBL, I will label it by unit or lab.

### Some Key Terms in Java:
- The main method is where the program starts running.
- Objects are an instance of a class. Objects can have attributes. For instance, a Student object might have name and grade as attributes.
- A class is a programmer defined blueprint from which objects are created.
    - Ex: Class is ClubMember
        - Attributes: Name, grade
- A parameter is a variable in the method/constructor signature that defines the type of value to receive when the method or constructor is called.
- An argument is a value passed to a method or constructor when the method or constructor is called.
- Super class is a class that can be extended to create subclasses
- Subclass is a class that extends a superclass and inherits its attributes and behaviors
- Inheritence is an OOP principle where a subclass inherits the attributes nad behaviors of a superclass
- Concatenation is joining two strings together

### 8/30 Using Objects
- Public means availible everywhere
- Final means that its not going anywhere
- myPainter.move();
    -  (.) notation means that you're using objects
    -  Refrencing data property or refrencing method
    -  myPainter is object
    -  .move(); is a method
    
### Unit 6 Inheritence

Instantiate an object
```
ClassName objectName = new ClassName();

// example
PainterPlus myPainterPlus = new PainterPlus();
```

Creating a subclass
```
public class Subclass extends SuperClass {

   public Subclass() {
      super();
   }
}
```

### Unit 7 Writing a Method

<img width="328" alt="Screen Shot 2022-09-05 at 2 23 43 PM" src="https://user-images.githubusercontent.com/89219525/188513554-ae1320d5-02e8-4f18-aa2f-26eee5d08b51.png">

```
public class PainterPlus extends Painter{
  public PainterPlus(){
    super();
  
  }
  public void turnRight(){
    turnLeft();
    turnLeft();
    turnLeft();
    
  }
  
}
```

//Unit 9 While Loops
Control Structure: A conditional or iteration statement which affects the flow of a program

<img width="681" alt="Screen Shot 2022-09-05 at 3 03 25 PM" src="https://user-images.githubusercontent.com/89219525/188515957-eb0074f5-091e-40c9-8fc4-c65e91a1e45b.png">

//Unit 10 Two Way Selection
Logical Operators
- Put in front of condition

NOT (!) - Returns opposite of operand 

```
 public void moveOrTakePaint(){
    while (canMove())  
      if (!isOnBucket()){
        move();
      }
      else
        takePaint();
    }
  
```

### Array List

- Arrays are used when you have a collection of the same type of elements
    - Ex: array of numbers, string array
- Arrays have a fixed size    
- ArrayLists don't have a fixed size, can change their size

### Unit 01 Primitive Types 

<img width="445" alt="Screen Shot 2022-10-16 at 7 29 49 PM" src="https://user-images.githubusercontent.com/89219525/196076377-d63059fa-77f8-48b2-946f-ad2bb39329f6.png">

Java Type Casting

Widening Casting (automatically): converting a smaller type to a larger type size
byte -> short -> char -> int -> long -> float -> double

Narrowing Casting (manually): converting a larger type to a smaller size type
double -> float -> long -> int -> char -> short -> byte

Java Operators

<img width="363" alt="Screen Shot 2022-10-16 at 7 32 23 PM" src="https://user-images.githubusercontent.com/89219525/196076719-03b61182-94da-4cfe-bc0e-d9bc7cf323e4.png">

Incrementing and Decrementing: ++ or --

### Unit 02 Using Objects

OOP (Object Oriented Programming): A programming paradigm that organizes software design around objects. 

<img width="279" alt="Screen Shot 2022-10-16 at 7 35 46 PM" src="https://user-images.githubusercontent.com/89219525/196077118-0b63f1c4-dbd2-4f24-8f07-e758c329dbee.png">

Classes: Templates/blueprints from which objects are creaeted. Objects under the same class with share common methods/attributes

     Ex: Class fruit can have the objects apple, bananas, and orange
     
     Ex: Class attributes (inherited by objects) could be calorie count, quantity, etc

Objects: Instances of a class

     Ex: Painter myPainter = new Painter();

Methods: Functions that perform a specific task

    Ex: Methods of the class could be store, cosume, etc

<img width="385" alt="Screen Shot 2022-10-16 at 7 39 46 PM" src="https://user-images.githubusercontent.com/89219525/196077565-376b293c-5a44-49d5-8063-aa5d7b76e01e.png">



