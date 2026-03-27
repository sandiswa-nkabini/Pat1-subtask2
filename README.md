# Pat1-subtask2
#include <iostream>
using namespace std;

int main() { 
    int temp1, temp2, temp3;
    int diff; 

    // Input first temperature
    cout << "Enter the first temperature reading: ";
    cin >> temp1;

    // Input second temperature
    cout << "Enter the second temperature reading: ";
    cin >> temp2;

    // Calculate difference
    diff = temp2 - temp1;

    // Check conditions for second reading
    if (diff > 50) {
        cout << "Reduce fryer heat before taking the third reading." << endl;
    }
    else if (diff < 10) {
        cout << "Increase fryer heat before taking the third reading." << endl;
    }

    // Input third temperature
    cout << "Enter the third temperature reading: ";
    cin >> temp3;

    // Final check for frying readiness
    if (temp3 >= 150 && temp3 <= 190) {
        cout << "You may start frying the Magwinyas." << endl;
    } else {
        cout << "Oil is not ready for frying!" << endl;
    }

    return 0;
}
