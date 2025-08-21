## what is this keyword in Java?
- this keyword always refers to current object(this object on which a method or constructor is being called).

## program

```
class Noc{
    //properties
    int num;
    //methods
    void addFive(){
        System.out.println("num="+(this.num+5));
    }
}
public class Main{
    public static void main(String[] args){
        Noc obj=new Noc();
        obj.addFive();
    }
}
```
```
o/p
num=5
```