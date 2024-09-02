# EXPERIMENT-11

## Aim :
To study and implement Classes and Objects

## Software :
Vs code

## Theory :

### Object Oriented Programming (OOP):
Object-oriented programming is based on the concept of objects. In object-oriented programming data structures, or objects are defined, each with its own properties or attributes.
To understand OOP better, let us understand some key concepts of OOPS
### classes :
A class is a user-defined data type, which holds its own data members and member functions, which can be accessed and used by creating an instance of that class.<br>A C++ class is like a blueprint for an object.
It defines a data structure by combining data (attributes) and methods (functions) that operate on the data. A class is defined using the class keyword followed by the class name and a block of code that includes its attributes and methods

**For Example:** Consider the Class of Cars. There may be many cars with different names and brands but all of them will share some common properties like all of them will have 4 wheels, Speed Limit, Mileage range, etc. So here, the Car is the class, and wheels, speed limits, and mileage are their properties.

- A Class is a user-defined data type that has data members and member functions.<br>
- Data members are the data variables and member functions are the functions used to manipulate these variables together, these data members and member functions define the properties and behaviour of the objects in a Class.<br>
- In the above example of class Car, the data member will be speed limit, mileage, etc, and member functions can be applying brakes, increasing speed, etc.

### objects :
An object is created from a class. We have already created the class named MyClass, so now we can use this to create objects.<br>
An instance of a class. It represents a specific realization of the class, holding actual values for the attributes defined by the class.An object is created by instantiating the class. This involves calling the class as if it were a function.

### Global and Local Variables
****Global Variables****:

Global variables are declared outside of functions or blocks, usually at the top of a program or in a separate file. They are accessible from any part of the program and retain their value throughout the program's lifetime. While useful for shared data, their widespread accessibility can lead to unintended side effects and make debugging more challenging, particularly in large programs. They are commonly used for values needed across multiple parts of the program
- **Declaration**: Outside of any function or block
- **Scope**: Entire program.
- **Usage**: Values that need to be accessed and modified by multiple parts of the program.
- **Lifetime**: Retain their value throughout the lifetime of the program

****Local Variables****:

Local variables are declared within a specific block of code, such as a function or loop. They are only accessible within that block and are released from memory when the block exits. Local variables can have the same name as those in other blocks without causing conflicts, as their scope is confined to their respective block. They are typically used for temporary storage or context-specific data.
- **Declaration**: Typically within functions or specific blocks
- **Scope**: Limited to the function or block where they are declared.
- **Usage**: Temporary storage, specific to a block of code
- **Lifetime**: Created when the block is entered and destroyed when it exits

## CODE - 
### A - 
#### Defining Class
```
#include <iostream>
using namespace std;

class Cube {
    public:
    double height = 2.0;
    double width = 3.0;
    double length = 5.0;  
};

int main() {
    Cube c1;
    double vol = c1.height * c1.width * c1.length;  
    cout << "Volume: " << vol << endl;
}
```

### B - 
#### Function inside a class
```
//Varun Pendem
// 2307023149
#include<iostream>
using namespace std;
class cube
{
    public:
    double height=3.0;
    double width=4.0;
    double length=5.0;

    double volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    double v = cube1.volume();
    cout<<"volume:"<<v<<endl;
}
```

### C - 
#### Public and Private variables
```
// Varun Pendem
// 23070123149

#include<iostream>
using namespace std;
//concept of public and private variables in class
class cube
{
    private:
    double height=4.0;
    double width=5.0;
    double length=6.0;

    public:
    double volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
};

int main()
{
    cube cube1;
    double v = cube1.volume();
    cout<<"volume:"<<v<<endl;
}
```

### D - 
#### Display fucntion inside a class
```
// Varun Pendem
// 23070123149
#include<iostream>
using namespace std;
//display function inside class
class cube
{
    public:
    double height=5.0;
    double width=6.0;
    double length=7.0;

    double volume()
    {
        double v;
        v=height*width*length;
        return v;
    }
    void disp_vol(double vol)
    {
        cout<<"volume :"<<vol<<endl;
    }
};
int main()
{
    cube cube1;
    double v = cube1.volume();
    cout<<"volume:"<<v<<endl;
    cube1.disp_vol(v);
}
```


## Outputs - 
### A -
<img width="325" alt="Screenshot 2024-09-01 at 2 25 45 AM" src="https://github.com/user-attachments/assets/265c17f9-6dad-453a-bb9b-c7319c3b9078">

### B -
<img width="344" alt="Screenshot 2024-09-01 at 2 26 17 AM" src="https://github.com/user-attachments/assets/d9d223e1-3196-412f-a1c9-d5599fcba35e">

### C - 
<img width="335" alt="Screenshot 2024-09-01 at 2 26 40 AM" src="https://github.com/user-attachments/assets/2d5f4f88-b30e-441b-a31b-ea8be6c4b606">

### D - 
<img width="374" alt="Screenshot 2024-09-01 at 2 28 10 AM" src="https://github.com/user-attachments/assets/84e99abe-8677-4513-9de4-ebe758e641ee">



## Conclusion - 
&#8594; We learnt about OOP in C++. <br>
&#8594; We learnt the use case of classes and objects in C++. <br>
*******
<br>
