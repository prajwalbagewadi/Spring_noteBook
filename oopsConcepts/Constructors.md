## Constructors ?
- Constructors are Special methods used to initialize objects.
- has the same name as the class.
- called automatically when you create an object using new keyword.
- does not have a return type.

## Types 

Default - If you do not create a constructor, java automatically provides one.

```
class NameOfClass {
    //constructor
    NameOfClass () {
        //default value assignment or initilization tasks 
    }
}
```
paramterized - used to assign user defined values to objects.

```
class NameOfClass {
    //properties
    dataType var;
    //constructor
    NameOfClass (dataType para,dataType para) {
        var=para;
    }
}
```

## program
```
class Dish{
    //properties
    private String dname;
    float dprice;

    //constructor
    Dish(){
        dname=null;
        dprice=0.00f;       
    }

    //overloaded.
    Dish(String name,float price){
        this.dname=name;
        this.dprice=price;
    }
    //methods
    
    void showDish(){
        System.out.println("Dish:");
        System.out.println("Dish Name:"+this.dname);
        System.out.println("Dish Price:"+this.dprice);       
    }
}

public class Main{
    public static void main(String[] args){
        //objects
        Dish d1=new Dish();
        Dish d2=new Dish("Margherita Pizza",400);

        //invoking class methods
        d1.showDish();
        d2.showDish();
    }
}
```
```
o/p
Dish:
Dish Name:null
Dish Price:0.0
Dish:
Dish Name:Margherita Pizza
Dish Price:400.0
```
