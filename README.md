# Prime-Check
Checks if given number is a prime number


{
#include <iostream>
#include <cmath>

using namespace std;

int main() {
    // Write your main here
    int num1;
// Prompts user input
    cout<<"Enter a positive integer: "<<endl;
    cin>> num1;
//Checks to see if number input is 2 and outputs result
    if (num1 == 2){
      cout<<"2 is a prime number"<<endl;
    }
//checks to see if number is positive
    if(num1 < 0){
      cout<<num1<<" is not a positive number.";
    }

// for loop runs to make sure the number entered is divisible by i value
    for(int i = 3; i <= sqrt(num1) ; i+= 2){
      if((num1 % i) == 0){
        cout<<num1<<" is not a prime number.";
        break;
      }



    }



    cout<<num1<<" is a prime number.";


    return 0;
}

}
