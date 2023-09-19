# StudentPayTax
C++ program taking hours a student worked at $7.50 an hour and calculating taxes and pay



    #include <iostream>
    using namespace std;

    int main(){
    const float TAXWITHHOLD = 0.15;
    const float PAY = 7.50;
    float hoursWorked;
    float taxWitheld;
    float netPay;
    float grossPay;


    hoursWorked = 0;
    taxWitheld = 0;
    netPay = 0;
    grossPay = 0;

    cout << "how many hours did you work this week?" << endl;
    cin >> hoursWorked;

    grossPay = PAY * hoursWorked;

    taxWitheld = grossPay * TAXWITHHOLD;

    netPay = grossPay - taxWitheld;

    hoursWorked = static_cast<int>(hoursWorked * 100) / 100.0;

    grossPay = static_cast<int>(grossPay * 100) / 100.0;

    taxWitheld = static_cast<int>(taxWitheld * 100) / 100.0;

    netPay = static_cast<int>(netPay * 100) / 100.0;

    cout << "your hours worked = " <<  hoursWorked << endl;
    cout << "your gross pay was = " << grossPay << endl;
    cout << "your withheld tax = " << taxWitheld << endl;
    cout << "your net pay = " <<  netPay << endl;

    



    return 0;
}
