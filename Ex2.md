# Ex.No:2
# Ex.Name:Write a CPP Program to overload a function to perform sum of two integers and sum of three integers
## Aim:
To write a CPP Program to overload a function to perform sum of two integers and sum of three integers

## Algorithm:
Start

Define a class Arithmetic with two overloaded member functions:

Add(int a, int b) → Calculates and prints the sum of two integers.

Add(float a, float b, float c) → Calculates and prints the sum of three floating-point numbers.

In the main() function:

Declare an object a of class Arithmetic.

Declare two integer variables a1 and a2.

Read two integer inputs from the user (cin >> a1 >> a2).

Call a.Add(a1, a2) to calculate and print their sum.

Declare three integer variables b1, b2, and b3.

Read three integer inputs from the user (cin >> b1 >> b2 >> b3).

Call a.Add(b1, b2, b3) → implicit type conversion occurs (integers promoted to floats) → calculates and prints the sum of three numbers.

End




## Program:
```
#include<iostream>
using namespace std;
class Arithmetic{
  public:
  void Add(int a,int b){
      cout << "Sum of two Numbers=" << a+b << endl;
  }
  void Add(float a,float b,float c){
      cout << "Sum of three Numbers=" << a+b+c;
  }
};
int main()
{
    Arithmetic a;
    int a1,a2;
    cin >> a1 >> a2;
    a.Add(a1,a2);
    int b1,b2,b3;
    cin >> b1 >> b2 >> b3;
    a.Add(b1,b2,b3);
    return 0;
}
```

## Output:

<img width="1329" height="269" alt="image" src="https://github.com/user-attachments/assets/4f64624a-17f8-44a6-8386-8b0e658c4176" />


## Result:
Hence the program is executed successfully.
