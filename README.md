# Reversing-a-String

/*This is a C++ Program to Reverse a String.
The program takes a string and reverses it.*/

#include <iostream>
#include <string.h>

using namespace std;

int main()
{
    char str[50], temp;
    int i, j;
    
    // The program takes a string.
    cout << "Enter a string : ";
    gets(str);
    
    // The string is copied into another string from backwards.
    j = strlen(str) - 1;
    
    // Using a for loop and string function, the string is reversed.
    for (i=0; i < j; i++, j--)
    {
        temp = str[i];
        str[i] = str[j];
        str[j] = temp;
    }
    
    // The result is printed.
    cout << "\nReverse String : " << str;
    
    // Exit.
    return 0;
}
