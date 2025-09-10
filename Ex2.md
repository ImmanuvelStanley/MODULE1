# Ex.No2
# Ex.Name:Write a C++ program to swap two names using class methods(method need to define outside class).

## Aim:
To write a C++ program to swap two names using class methods(method need to define outside class).

## Algorithm:
1. Start
2. Read first name
3. Read second name
4. Display names before swapping
5. Swap names using class method
6. Display names after swapping
7. Stop

## Program:
```
#include <iostream>
#include <string>
using namespace std;

class NameSwapper {
private:
    string name1, name2;

public:
    void setNames(string n1, string n2);
    void swapNames();
    void displayNames();
};

// Method definitions outside the class
void NameSwapper::setNames(string n1, string n2) {
    name1 = n1;
    name2 = n2;
}

void NameSwapper::swapNames() {
    string temp = name1;
    name1 = name2;
    name2 = temp;
}

void NameSwapper::displayNames() {
    cout << "After swapping the 1st name is:" << name1 << endl;
    cout << "After swapping the 2nd name is:" << name2 << endl;
}

int main() {
    NameSwapper obj;
    string first, second;

    cin >> first >> second;
    
    obj.setNames(first, second);
    obj.swapNames();
    obj.displayNames();

    return 0;
}
```




## Output:
<img width="1180" height="385" alt="Screenshot 2025-09-10 102249" src="https://github.com/user-attachments/assets/716d6fab-4e06-454f-92fd-bb3ece418d54" />

## Result:
The program successfully generates to swap two names using class methods.
