# EXP-9

## Aim:
**To study and implement Pointer Operations (Call by value and Call by reference)..**

## Software:
`Microsoft VSCode`

## Theory:
Pointers are symbolic representations of addresses.
We can pass arguments to funtions using different methods mainly call by value and call by reference.

Call by value
In the call-by-value method, function arguments are passed by copying the value of the actual parameter, ensuring the original values remain unchanged.
The value is copied to the formal parameter.
Any changes made to the parameters within the function do not change the original values outside the function.

Call by reference
In the call-by-reference method, the memory address (reference) of the actual parameter is passed to the function, allowing direct access and modification of the original values.
The actual and the formal parameters point to the same memory address.

Any changes made to the parameters within the function are directly reflected in the original values outside the function.
## Code: 10A
```
//KANWALJEET SINGH
//ENTC B2
//EXP 10A
//23070123124
// // Printing the values by using callby value 

#include<iostream> 
using namespace std; 
void swap(int x, int y) 
{
    int swap;
    swap=x;
    x=y;
    y=swap;
}

int main() 
{
    int a=4, b=7;
    swap(a,b);
    cout<<"Value of a is: "<<a<<"\n";
    cout<<"Value of b is: "<<b<<"\n";
    return 0;
}
```
## Output:
![image](https://github.com/user-attachments/assets/ebe09b84-dc8e-4468-88ef-89e0551be0f1)






## Code: 10B
```
//KANWALJEET SINGH
//ENTC B2
//EXP 10B
//23070123124
// Swapping the values 

#include<iostream> 
using namespace std; 
void swap(int *x, int *y) 
{
    int *swap;
    swap=x;
    x=y;
    y=swap;
}

int main() 
{
    int a=4,b=7;
    swap(a,b);
    cout<<"Value of a is: "<<a<<"\n";
    cout<<"Value of b is: "<<b<<"\n";
    return 0;
} 
```

## Output:
![image](https://github.com/user-attachments/assets/5ccb286c-8bfd-4ba1-90b9-f60c6a2a496b)


## Code:10C
```
//KANWALJEET SINGH
//ENTC B2
//EXP 10C
//23070123124
// Swapping the values using call by reference  

#include<iostream> 
using namespace std; 
void swap(int *x, int *y) 
{
    int swap;
    swap=*x;
    *x=*y;
    *y=swap;
}

int main() 
{
    int a=4,b=7;
    swap(&a,&b);
    cout<<"Value of a is: "<<a<<"\n";
    cout<<"Value of b is: "<<b<<"\n";
    return 0;
}
```

## Output: ![image](https://github.com/user-attachments/assets/d94fef51-564f-4230-a2d7-01154a89452c)

### Conclusion:
I learnt about pointers and how to pass arguments to functions using call by value and call by reference methods. I also learnt how to swap values using call by reference.
