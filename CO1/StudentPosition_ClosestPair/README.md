

## Description

This project contains a Python script that determines the proximity of students based on their 2D coordinate positions. It implements a closest pair algorithm (using Euclidean distance) to analyze a set of student coordinates and identify the two students who are standing closest to each other.

## Algorithm

The core logic of the system follows this step-by-step algorithm:

1. **Start**
2. **Initialize Data:** Define a list of students and their corresponding (X, Y) coordinate positions.
3. **Display Positions:** Print the current positions of all students.
4. **Calculate Distances:** Iterate through all possible pairs of students and calculate the Euclidean distance between them.
5. **Find Minimum:** Compare the calculated distances to find the smallest value, keeping track of the two students associated with that minimum distance.
6. **Display Result:** Print the names of the two closest students and the distance between them.

## Input and Output



--- Student Positions ---<br>
Ravi : (2, 3)<br>
Sita : (10, 15)<br>
John : (4, 5)<br>
Anu : (20, 25)<br>
Rani : (8, 12)<br>
<br>
--- Closest Students ---<br>
Students: Ravi and John<br>
Distance: 2.83
