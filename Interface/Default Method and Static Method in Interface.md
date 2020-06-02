# Default Method and Static Method in Interface

- In Java8, We can define the method in interface by using **default** keyword.

#### For example:

``` 
interface I{

default void show(){
        System.out.println("Hello");
    }
}
```

- when we implement the interface in class then there is no need to define the body of method we can access like:

lets suppose there is a Class **A**
```
A obj = new A();
obj.show(); // no need to define the body.

```

###### Lets Take another scenario

- Suppose We have 2 interface **I** and **J** and both interface have same method using **default** keyword like **show()**. Now We implement one interface **I** in class **A** then no need to define the method. We can directly access like:
```
A obj = new A();
obj.show();

```
- But we implements both interface **I** and **J** then problems arise and compiler gives an error so we have a solution over here that is We have to define that method in a class **A**.  


###### Lets take one more scenario

- suppose we have two interface **I** and **J** and both interface have same code like:

```
interface I{

default void show(){
        System.out.println("Hello");
    }
}

interface J{

default void show(){
        System.out.println("Hii");
    }
}
```

> Now Create a class A and having same method **show()**

```
class A{

public void show(){
        System.out.println("Class A Show");

    }
}
```
> Now Create a class C which are extends by class **A** and implements by interfaces **I** and **J**.

```
public class C extends A implements I,J{

}
```
Now create an object of class **C** which method will call .

```
C obj = new C();
obj.show(); 
```

here class **A** method will call because Class is more powerful than interface or Normal Method is higer priority than default method of interface.
so output is : **Class A show**


#### Static Method in Interface
- Static methods in interfaces which can be called independently without an object. Note: these methods are not inherited.

```
interface I{
    static void show();
}
```
- to call this static method you can directly call in Main Function like:

```
I.show();

```

#### Note:
- Default or Static method can only be used with java 1.8 version.
