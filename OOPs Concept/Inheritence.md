# Inheritence in JAVA

## Inheritence:

- All the members of parent class is the member of child class by birth.
- One subclass(child class) can extend only one super class in Java but it can implement the multiple interfaces.
- A private member of the super class can not be inherited in subclass e.g. private field and private methods.
- Default member can only be inherited in same package subclass, not in another package.
- The **constructor** in Java is not inherited by the subclass.
- If a class implements Interface or extends an abstract class, it needs to override all abstract methods until it is not abstract.
- Multiple inheritances are not supported in java but we can achieve this by using interface. One class can implement multiple interfaces.
- In Java, class never extends the interface rather it implements interface
- One interface can extend another interface in Java.

#### For Example:
**1.**
```
class A{
    int num1, num2, result=0;
    
   public void sum(){
       result = num1+num2;
   }
}

class B extends A{

public void sub(){
       result = num1-num2;
   }
}
```
This is called **Single Level Inheritence.**

**2.**

```
class A{
    int num1, num2, result=0;
    
   public void sum(){
       result = num1+num2;
   }
}

class B extends A{

public void sub(){
       result = num1-num2;
   }
   
class C extends B{

public void Multi(){
       result = num1*num2;
   }
}
```
This is called **Multi Level Inheritence.**


