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





