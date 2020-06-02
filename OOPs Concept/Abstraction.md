# Abstraction in JAVA

## Abstract Class:

- An abstract class may or may not have all abstract methods. Some of them can be concrete methods
- But method is abstract then class must be abstract class.
- Any class that contains one or more abstract methods must also be declared with abstract keyword.
- There can be no object of an abstract class.
- An abstract class can have parametrized constructors and default constructor is always present in an abstract class.
- An abstract class may have static fields and static methods.


#### Example:

```
public abstract class A { // Abstract Class
 
 public void show(String Message){
        System.out.println(message);
 }
 
 public abstract void print(); // Abstract Method
 
}


now create non Abstract class which extends Abstract class(A):

public class B extends A{ // Concrete Class
	
	@override
	public void show(String message) {
    super.show(message);
	}
	
	@Override
	public void print() {

    show("Hello !!!");
  }
}
```

#### Conclusion:

- Abstract method of abstract class must be Override in Derived class.
- Non abstract method of abstract class always call method of Super class.
