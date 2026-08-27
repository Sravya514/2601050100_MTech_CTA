

## Description

This project contains a Python script that analyzes a sequence of temperature fluctuations. It implements a Maximum Subarray algorithm to identify the contiguous period of days that results in the highest overall net change in temperature.

## Algorithm

The core logic of the system follows this step-by-step algorithm:

1. **Start**
2. **Initialize Data:** Define an array representing a sequence of daily temperature changes.
3. **Process Subarrays:** Iterate through the array to calculate running totals of the temperature changes.
4. **Track Maximums:** Keep track of the highest total change encountered and the specific start and end indices of that sub-period.
5. **Extract Best Period:** Use the optimal start and end indices to slice the original array, isolating the "Best Weather Period."
6. **Display Results:** Print the original sequence, the contiguous sub-sequence with the maximum sum, and the calculated maximum total change.

## Input and Output

### Input


`[3, -1, 4, 2, -2, 5, -6]`

### Output

Temperature Changes: [3, -1, 4, 2, -2, 5, -6]<br>
Best Weather Period: [3, -1, 4, 2, -2, 5]<br>
Maximum Change: 11
