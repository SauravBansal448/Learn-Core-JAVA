# Polymorphism in JAVA

## Polymorphism:
 In Polymorphism, There are 2 Concepts:

- Method Overloading
- Method OverRiding

## Method Overloading:

- In Method Overloading, In a class, there can be multiple numbers of methods, methods name is same but it have different number or types of parameters.
- It is also called compile-time polymorphism, early binding, static binding.
- Overloaded methods are fast because they are bonded during compile time and no check or binding is required during runtime
 
#### For Example:

```
class A{

public void show(){

}

public void show(int i){

}

public void show(float f){

}

public void show(int j, float g){

}
}
```

## Method OverRiding:

- In Method Overriding, Method name is same, same number of parameters but in diffrent class.
- It is also called run-time polymorphism, late binding, dynamic binding.


#### For Example:

```
class A{

public void show(){

    }
}

class B{

public void show(){

    }
}
```
