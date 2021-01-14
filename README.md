# inverse-odd-factorials

#include <iostream>
using namespace std;


int main(){
    int n;
    cout << "Enter the value of N: ";
    cin >> n;
    cout << 1;
    for(int i=3; i<=n; i+=2){
        cout << "+ (1/" << i << "!) ";
    }

    cout << "= ";

    float sum = 0;

    for(int i=1; i<=n; i+=2){
        int s = 1;
        for(int j=1; j<=i; j++){
                s = j*s;
        }
        sum = sum + (1.0/s);
    }
    cout << sum;
    return 0;
}
