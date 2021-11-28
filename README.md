# Lesson-14
// Lesson 14.cpp : This file contains the 'main' function. Program execution begins and ends there.
//

#include <iostream>
#include <array>
#include <algorithm>
using namespace std;
int main()
{
    array<string, 4> arr = { "Mars Bars", "Snickers", "Bounty", "Wispa" };
    cout << arr.at(1) << endl;
    cout << arr[1] << endl;
    cout << arr.front() << endl;
    cout << arr.back() << endl;
    for (int i = 0; i < arr.size(); i++) {
        cout << arr.at(i) << ", ";
    }
    cout << endl;
    cout << "This code will print Algorithm Sorting Example:\n";
    {
        array<int, 5> numbers = { 33, 5, 7, 99, 83 };
        sort(numbers.begin(), numbers.end());
        for (int num : numbers) {
            cout << num << "  ";
        }
    }
    cout << "\nThis code will print rand funtion:\n";
    int randomArry[10];
    for (int i = 0; i < 10; i++) {
        randomArry[i] = rand() % 50;
        cout << randomArry[i] << endl;
    }
}

// Run program: Ctrl + F5 or Debug > Start Without Debugging menu
// Debug program: F5 or Debug > Start Debugging menu

// Tips for Getting Started: 
//   1. Use the Solution Explorer window to add/manage files
//   2. Use the Team Explorer window to connect to source control
//   3. Use the Output window to see build output and other messages
//   4. Use the Error List window to view errors
//   5. Go to Project > Add New Item to create new code files, or Project > Add Existing Item to add existing code files to the project
//   6. In the future, to open this project again, go to File > Open > Project and select the .sln file
