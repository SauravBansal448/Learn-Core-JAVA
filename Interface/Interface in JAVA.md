# Interface in Java

## Interface

- To declare an interface, use interface keyword. It is used to provide total abstraction.
- We can’t create object(interface can’t be instantiated) of interface.
- It is used to achieve multiple inheritence.
- By default all the methods in interface is abstract methods.
- Like a class, an interface can have methods and variables, but the methods declared in an interface are by default abstract (only method signature, no body).

#### Why do we use interface ?
- Since java does not support multiple inheritance in case of class, but by using interface it can achieve multiple inheritance.
- It is used to achieve total abstraction.
- Interfaces are used to implement abstraction. So the question arises why use interfaces when we have abstract classes?
    **The reason is, abstract classes may contain non-final variables, whereas variables in interface are final, public and static.**

#### For Example:

```
interface display(){

void show(String Message);

}

> Now Create a class 

class A implements display{ 

@override
public void show(String message){
        System.out.println(message);
    }
}
```

