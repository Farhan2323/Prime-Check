# Prime-Check
//Checks if given number is a prime number



#include <iostream>
#include <cmath>

using namespace std;

int main() {
    // Write your main here
    int num1;

    cout<<"Enter a positive integer: "<<endl;
    cin>> num1;

    if (num1 == 2){
      cout<<"2 is a prime number"<<endl;
    }

    if(num1 < 0){
      cout<<num1<<" is not a positive number.";
    }


    for(int i = 3; i <= sqrt(num1) ; i+= 2){
      if((num1 % i) == 0){
        cout<<num1<<" is not a prime number.";
        break;
      }



    }



    cout<<num1<<" is a prime number.";


    return 0;
}


