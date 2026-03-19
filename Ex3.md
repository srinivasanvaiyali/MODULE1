# Ex.No:3
# Ex.Name:Write a C++ program to read the product details using the constructor and display them using a member function.
## Date:
## Aim:
To write a C++ program that reads product details such as product name, brand, and product serial number using a constructor, and displays them using a member function.

## Algorithm:
1.Start the program.

2.Define a class with private data members to store product details (name, brand, and serial number).

3.Create a parameterized constructor to initialize these details.

4.Define a member function to display the product details on the screen.

5.Read product details from the user, create an object using the constructor, and call the member function to display the details.



## Program:
```
#include<iostream>
using namespace std;
class uu
{
    public:
    uu(string a,string b,string c)
    {
        cout<<"Product name is "<<a<<endl;
        cout<<"Brand is "<<b<<endl;
        cout<<"Product serial number is "<<c;
    }
};
int main()
{
    string a,b,c;
    
    cin>>a>>b>>c;
    uu o(a,b,c);
}
```


## Output:

<img width="1187" height="488" alt="484043267-0249a06d-9b1d-4461-9da2-fec8f7598b92" src="https://github.com/user-attachments/assets/7b479f65-c6d5-4c98-be9a-c6a267e0e2d3" />


## Result
Thus a C++ program to read the product details using the constructor and display them using a member function has been executed successfully.
