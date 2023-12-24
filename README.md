- 👋 Hi, I’m @Krishnachavan1930
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Krishnachavan1930/Krishnachavan1930 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
You can create a C++ program to convert temperatures between Fahrenheit and Celsius using the following code:
#include <iostream>
using namespace std;

// Function to convert Fahrenheit to Celsius
double fahrenheitToCelsius(double fahrenheit) {
    return (fahrenheit - 32.0) * 5.0 / 9.0;
}

// Function to convert Celsius to Fahrenheit
double celsiusToFahrenheit(double celsius) {
    return (celsius * 9.0 / 5.0) + 32.0;
}

int main() {
    char choice;
    double temperature;

    cout << "Temperature Conversion Menu" << endl;
    cout << "1. Fahrenheit to Celsius" << endl;
    cout << "2. Celsius to Fahrenheit" << endl;
    cout << "Enter your choice (1 or 2): ";
    cin >> choice;

    if (choice == '1') {
        cout << "Enter temperature in Fahrenheit: ";
        cin >> temperature;
        cout << temperature << " Fahrenheit is " << fahrenheitToCelsius(temperature) << " Celsius" << endl;
    } else if (choice == '2') {
        cout << "Enter temperature in Celsius: ";
        cin >> temperature;
        cout << temperature << " Celsius is " << celsiusToFahrenheit(temperature) << " Fahrenheit" << endl;
    } else {
        cout << "Invalid choice!" << endl;
    }

    return 0;
}


