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
