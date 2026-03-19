# Ex.No:5
# Ex.Name:Write a C++ program using friend function to find the minimum integer value  among the member of both the classes.
## Date:
## Aim:
To write a C++ program that demonstrates the use of a friend function to access private data members of two different classes and find the minimum integer value among them.

## Algorithm:
1.Start the program.

2.Define two classes (ClassA and ClassB) with private integer members.

3.Declare a friend function in both classes so it can access their private members.

4.Implement the friend function findMinimum() to compare the integer values of both classes.

5.Read integer values, create objects of both classes, and call the friend function to display the minimum value.



## Program:
```
#include <iostream>
using namespace std;

class ClassB; // Forward declaration

class ClassA {
    int valueA;
public:
    ClassA(int val) { valueA = val; }
    friend void findMinimum(ClassA, ClassB);
};

class ClassB {
    int valueB;
public:
    ClassB(int val) { valueB = val; }
    friend void findMinimum(ClassA, ClassB);
};

void findMinimum(ClassA objA, ClassB objB) {
    if (objA.valueA < objB.valueB) {
        cout << "Minimum value is " << objA.valueA << endl;
    } else {
        cout << "Minimum value is " << objB.valueB << endl;
    }
}

int main() {
    int a, b;
    cin >> a;
    cin >> b;
    
    ClassA objA(a);
    ClassB objB(b);
    
    findMinimum(objA, objB);
    
    return 0;
}
```


## Output:

<img width="1176" height="412" alt="484044958-b2e777f0-52b8-4730-856f-0706c2b39f96" src="https://github.com/user-attachments/assets/18ee6cb9-5719-4ff6-aac2-b91ce4034223" />


## Result:
Thus the C++ program using friend function to find the minimum integer value among the member of both the classes has been executed successfully.
