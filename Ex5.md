# Ex.No:5
# Ex.Name:Write a C++ program to convert Celsius into Fahrenheit using inline function  

## Aim:
To write a C++ program to convert Celsius into Fahrenheit using inline function  

## Algorithm:
1. Start
2. Define an inline function to convert Celsius to Fahrenheit
3. Formula: Fahrenheit = (Celsius × 9/5) + 32
4. Declare main() function
5. Read Celsius temperature from user
6. Call inline function with Celsius value
7. Display the converted Fahrenheit temperature
8. Stop

## Program:
```
#include <iostream>
using namespace std;


inline double celciustofahreheit(double celcius)
{
    return (celcius *9.0/5.0)+32;
}

int main()

{
    double celcius;
    cin>>celcius;
    double fahrenheit=celciustofahreheit(celcius);
    cout<<"temperature in Fahrenheit:"<<fahrenheit<<endl;
    

    
}
```


## Output:
<img width="1015" height="259" alt="Screenshot 2025-09-10 104300" src="https://github.com/user-attachments/assets/7e92b323-4dc9-43e8-9c33-c19e18d6d2a5" />


## Result:
The program successfully converts Celsius into Fahrenheit using an inline function in C++.
