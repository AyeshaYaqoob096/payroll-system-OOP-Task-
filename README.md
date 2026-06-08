# Employee Payroll System

A lightweight C++ console application designed using Object-Oriented Programming (OOP) principles to calculate and manage weekly gross pay for employees. The program instantiates an array of custom class objects and enforces strict input validation boundaries to ensure data integrity.

---

## 🚀 Features

* **Object-Oriented Design:** Implements a robust `Payroll` class utilizing encapsulation, private data members, and public setter/getter methods.
* **Array of Objects:** Dynamically manages records for multiple employees simultaneously using structured object arrays.
* **Strict Input Validation:** Protects system logic by explicitly rejecting:
  * Overtime hours exceeding **60 hours** per week.
  * Negative values for both hours worked and hourly pay rates.
* **Clean Terminal Output:** Displays formatted weekly gross pay summaries for all processed employees.



## 🛠️ Tech Stack & Concepts

* **Language:** C++ (C++11 or higher recommended)
* **Paradigm:** Object-Oriented Programming (OOP)
* **Key Concepts:** Encapsulation, Defensive Programming, Input Streams, Data Validation, Array Traversal.



## 📋 Code Preview & Validation Logic

The core constraint of the application checks boundaries dynamically before modifying object states:

```cpp
// Input Validation: Restricting acceptable weekly hours
while (hours < 0 || hours > 60)
{
    cout << "Hours must be between 0 and 60. Enter again: ";
    cin >> hours;
}
