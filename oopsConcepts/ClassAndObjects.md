## what is class ?
- class is like a blueprint or template.
- It defines the properties(variables) and behaviours(methods).

```
syntax:
class NameOfClass {
    //properties
        int num;
    
    //constructor
    NameOfClass(int para){
        num=para;
    }

    //methods
    void dispNum(){
        System.out.println("num="+num);
    }
}
```

## what is an object ?
-   object is a real instance of class. 

```
syntax:
public static void main(String[] args){
    //                memory alloc  callTo Constructor   
    NameOfClass obj = new NameOfClass(int para);
}
```
- new keyword used to allocate memory followed by constructor call.

## Program
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

    //methods
    void addDish(String name,float price){
        this.dname=name;
        this.dprice=price;
    }

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
        Dish d2=new Dish();

        //invoking class methods
        d1.addDish("Margherita Pizza",400);
        d2.addDish("French Fries",100);
        d1.showDish();
        d2.showDish();
    }
}
```

```
o/p:
Dish:
Dish Name:Margherita Pizza
Dish Price:400.0
Dish:
Dish Name:French Fries
Dish Price:100.0
```
