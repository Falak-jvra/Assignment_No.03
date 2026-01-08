#include <iostream>
using namespace std;

void determineScholarship(int marks, float attendance) {
    if (marks >= 85) {
        if (attendance >= 80) {
            cout << "Full Scholarship" << endl;
        } else {
            cout << "Partial Scholarship" << endl;
        }
    } else {
        if (marks >= 70) {
            cout << "Partial Scholarship" << endl;
        } else {
            cout << "No Scholarship" << endl;
        }
    }
}

int main() {
    int marks;
    float attendance;
    double income;

    cout << "Enter Marks: ";
    cin >> marks;

    cout << "Enter Attendance: ";
    cin >> attendance;

    cout << "Enter Family Income: ";
    cin >> income;

    determineScholarship(marks, attendance);

    return 0;
}
