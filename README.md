# C-code For Fibonacci Series 
C++ code for 
#include <iostream>
using namespace std;

int main() {
    int n;
    cin >> n;

    int a = 0, b = 1;

    for (int i = 0; i < n; i++) {
        cout << a << " ";
        int next = a + b;
        a = b;
        b = next;
    }

    return 0;
}

# C-code For  Factorial Recursion 

#include <iostream>
using namespace std;

long long int fact(int n);

int main()
{
int n;
long long int factorial = 1;

cout << "Enter value: ";
cin >> n;

factorial = fact(n);

cout << "Factorial of " << n << " is " << factorial;

return 0;

}

long long int fact(int n)
{
if (n == 0 || n == 1)
return 1;
else
return (long long int)n * fact(n - 1);
} 
