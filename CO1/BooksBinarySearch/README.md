# Books Binary Search

## Description

This project contains a Python script that implements the **Binary Search algorithm** to find a specific book in a virtual library. The library is represented by a list of numbers ranging from **1 to 1,000,000**.

## How It Works

The code uses a function called `Library(target)` to perform the search. It takes the target book number as input and searches for it using the binary search method.

The algorithm:

* Sets `low` and `high` pointers to define the search boundaries.
* Calculates the `mid` point between `low` and `high`.
* Compares the value at `mid` with the target.
* If the book is found, it returns the index of the book.
* If the target is smaller than the middle value, it searches the left half.
* If the target is larger than the middle value, it searches the right half.
* If the book is not found, it returns `-1`.

## Usage

When the script is executed it prompts the user with:


What book do you want to find:

The user must enter an integer. The program then prints the index position of the book if it is found. Otherwise it displays a **book not found** message.

## Input and Output

### Input
What book do you want to find: 7500

### Output
Book at: 7499


