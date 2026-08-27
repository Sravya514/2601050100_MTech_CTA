
# Books Binary Search

## Description
This project contains a Python script that implements a binary search algorithm to find a specific book within a virtual library. The library is represented by a list of numbers ranging from 1 to 1,000,000. 

## How It Works
The code uses a function called `Library(target)` to perform the search. It takes the target book number as input and searches through the array using the binary search method:
* It sets `low` and `high` pointers to track the search boundaries.
* It calculates the `mid` point and compares it to the target.
* If the book is found, it returns the index position of the book.
* If the book is not found after narrowing down the search, it returns -1.

## Usage
When the script is executed, it prompts the user with the question: "what book do you want to find:". The user must enter an integer. The program will then print either the location index of the book (e.g., "book is at: 74999") or a "book not found" message.

## Output
Below are the output images demonstrating the execution and results of the program:

<img width="419" height="304" alt="image" src="https://github.com/user-attachments/assets/97c31220-d497-4133-aa3a-c2cf29602f66" />
