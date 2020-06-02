# Exception in Java

- An exception is an unwanted or unexpected event, which occurs during the execution of a program i.e at run time, that disrupts the normal flow of the program’s instructions.
- **Throwable** class is used to handle all the exceptions.
- **Throwable** class is extended by 2 main class that are:
    - Exception 
    - Error

## Types of Exceptions:

- **Checked Exception** also called compile time exception. eg. IOException, SQLException etc.
- **Unchecked Exception** also clled run time exception. eg. ArrayIndexBoundException, AirthmaticException etc.


#### Exception Handling in JAVA

###### Using try/catch

```
public class A{
int i=2,j=0,res=0;
res= i/j; 
System.out.println(res); // it Will throw the Airthmatic exception 
}

> To solve this exception we can put critical code in try block like:

public class A{
int i=2,j=0,res=0;
try{
res= i/j;
}catch(Exception e){
System.out.println("can not divide by zero.")
}
System.out.println(res);
}
```

#### Throws Keyword

- It is used to supress the exception not handling
- throws is a keyword in Java which is used in the **signature of method** to indicate that this method might throw one of the listed type exceptions. The caller to these methods has to handle the exception using a try-catch block.

#### For Example:

```
public void calculator() throws IOException{

}
```

#### Throw Keyword

- The throw keyword in Java is used to explicitly throw an exception from a method or any block of code. We can throw either checked or unchecked exception. 

#### For Example:

```
public void calculator() {

try{
    throw new AirthmaticException(); 
    
}catch(Exception e){
    System.out.println("Caught inside calculator()."); 
    throw e; // rethrowing the exception 
    
    }
}
```

#### Finally Keyword

- when any exception comes then execution of the code is directly jump to catch block but we want to execute some code either exception exists or not then we write a finally block to execute the code.

#### For example:

```
try{
res = i/j;
}catch(Exception e){
    System.out.println("Can't divide by zero");
}
finally{
    System.out.println("Byeee");
}

> Output : Can't divide by zero
            Byeee
            
```
