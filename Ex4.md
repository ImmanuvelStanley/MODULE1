# Ex.No:4
# Ex.Name:Write a C++ program using friend function to find the maximum integer value among the member of both the classes.

## Aim:
To write a C++ program using friend function to find the maximum integer value among the member of both the classes.


## Algorithm:
1. Start
2. Define two classes (ClassA and ClassB) with integer data members
3. Declare a friend function in both classes
4. Use constructors to initialize data members
5. Define the friend function outside the classes to compare values
6. In main(), read integer values from the user
7. Create objects of both classes and call the friend function
8. Display the maximum value and Stop


## Program:
```
#include <iostream>
using namespace std;

class ClassB;

class ClassA
{
private:
    int numA;

public:
    void setNumA(int num) 
    {
        numA = num;
    }

    friend void findMax(ClassA objA, ClassB objB);
};

class ClassB 
{
private:
    int numB;

public:
    void setNumB(int num)
    {
        numB = num;
    }

    friend void findMax(ClassA objA, ClassB objB);
};

void findMax(ClassA objA, ClassB objB) 
{
    cout << "Maximum value is " << (objA.numA > objB.numB ? objA.numA : objB.numB) << endl;
}

int main()
{
    int num1, num2;

    cin >> num1;

    cin >> num2;

    ClassA objA;
    ClassB objB;

    objA.setNumA(num1);
    objB.setNumB(num2);

    findMax(objA, objB);

    return 0;
}
```



## Output:
<img width="972" height="343" alt="Screenshot 2025-09-10 103418" src="https://github.com/user-attachments/assets/04ae241e-af5f-4b56-946b-00bcb7065041" />


## Result:
The program successfully created to find the maximum integer value.
