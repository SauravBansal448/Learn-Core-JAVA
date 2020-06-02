# Constructor in JAVA

## Constructor:
        
- Constructor is a member method.
- It has a same name as a Class Name.
- Main use of Constructor is that, what actual memory is required by an object. so this answer is given by the Constructor
- It will allocate the memory to the object.
- It is also used to initialise the variables.
- Constructor will never return anything so there is no need to write any return type(void, int etc).


#### For Example:

```
public class A{

int i;

public A(){     // this is a default constructor
    System.out.println("Hello");
  }    
  
  public A(int k){     // this is a Parameterised Constructor
    System.out.println("Hii");
  }    
}
```

#### How Constructor works in JAVA

- You can use public, private, protected access modifier with constructor or can even leave them without any parameter in that case it will use default access, which is at package-private level. 
- Private constructor are special, because if you make your constructor private, then no one can call it from outside that class, which means no external way to create instance of that class. If you make that private, it will not be accessible on child class and compiler will throw error. 
- Private constructor has another special use, in singleton design pattern, where goal is to keep just one instance of that class. Singleton creates instance by itself, caches it and provides a getInstance() method to make that instance available to outside world.

#### Note:
- More then one Constructor in a class with diffrent signature is called **Constructor Overloading**.
- You can't call constructor explicitly. **For Example:** 
``` 
A obj = new A(); // A() is a constructor.
obj.A(); //it gives an error
```

- Constuctor is called by **JVM** automatically when you create an object.
- There is no need to write default constructor.
- Super class constructor is executed before subclass


