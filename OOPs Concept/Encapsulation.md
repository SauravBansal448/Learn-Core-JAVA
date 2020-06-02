# Encapsulation in JAVA

## Encapsulation: 

- Encapsulation means hiding details of implementation from outside world so that when things change no body gets affected.
- Variables should be private.
- To access these varibales in main function then we have to implement getter and setter method.
- Encapsulation is implemented using private, package-private and protected access modifier
- Encapsulation is also called data hiding.
- Encapsulation allows you to change one part of code without affecting other parts of code.

#### For Example:

```
class Loan{
  
    private String loan;  //private variables examples of encapsulation
   
    //public constructor can break encapsulation instead use factory method
    private Loan(int loan){
        this.loan = loan;
    }
   
    //no argument constructor omitted here
    
   // create loan can encapsulate loan creation logic
    public Loan createLoan(String loanType){
  
     //processing based on loan type and then returning loan object
      return loan;
    }
   
}
```


