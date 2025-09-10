# Ex.No:3
# Ex.Name:Write a C++ program to read the product details using the constructor and display them using a member function.

## Aim:
To write a C++ program to read the product details using the constructor and display them using a member function.


## Algorithm:
1. Start
2. Define a class Product with data members (ID, Name, Price)
3. Declare a constructor to read product details from the user
4. Declare a member function to display product details
5. In main(), create an object of the class Product
6. Invoke the constructor automatically to read input
7. Call the member function to display product details
8. Stop

## Program:
```
#include <iostream>
#include <string>
using namespace std;

class Product 
{
private:
    string productName;
    string brand;
    int serialNumber;

public:
    Product(string name, string b, int serial) 
    {
        productName = name;
        brand = b;
        serialNumber = serial;
    }

    void displayDetails()
    {
        cout << "Product name is " << productName << endl;
        cout << "Brand is " << brand << endl;
        cout << "Product serial number is " << serialNumber << endl;
    }
};

int main() 
{
    string name, brand;
    int serial;

    cin>>name;
    cin>>brand;
    cin >> serial;

    Product obj(name, brand, serial);
    obj.displayDetails();
}
```



## Output:
<img width="1143" height="412" alt="Screenshot 2025-09-10 102846" src="https://github.com/user-attachments/assets/c541ccc2-ccc5-4ce9-929f-62f49b75fb74" />

## Result
The program successfully created to read the product details using the constructor and display them using a member function.

