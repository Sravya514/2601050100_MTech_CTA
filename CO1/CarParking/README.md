
# Parking Management System

## Description

This project contains a Python-based **Parking Management System** that manages vehicle entry, parking slot allocation, vehicle exit, and parking fee calculation.

The system has **100 parking slots** and automatically assigns the first available slot to each vehicle. It also records the vehicle's entry time and calculates the parking fee when the vehicle exits.

## How It Works

The program uses dictionaries and sets to manage the parking area:

* `parking_slots` stores information about each parking slot and the vehicle occupying it.
* `active_vehicles` keeps track of vehicles that are currently parked and their assigned slots.
* `available_slots` stores all currently available parking slots.
* When a vehicle enters, the system assigns the **lowest-numbered available slot**.
* The vehicle's entry time is recorded automatically.
* When a vehicle exits, the system calculates the parking duration.
* The parking fee is calculated at **20 currency units per hour**.
* A minimum of **1 hour** is charged, even if the vehicle stays for less than an hour.
* When a vehicle leaves, its parking slot becomes available again.

## Features

* Display available parking slots
* Automatically allocate parking slots
* Prevent the same vehicle from being parked twice
* Record vehicle entry time
* Calculate parking duration
* Calculate parking fees
* Release parking slots when vehicles exit
* Detect when the parking area is full
* Validate vehicle numbers and menu choices

## Configuration

The parking capacity and hourly rate can be changed using these variables:

```python
TOTAL_SLOTS = 100
RATE_PER_HOUR = 20
```

For example, changing `TOTAL_SLOTS` to `200` will create 200 parking slots.

## Usage

When the program is executed, it displays the following menu:

```text
--- Parking Management System ---
1. Display Availability
2. Vehicle Entry
3. Vehicle Exit
4. Exit Program
```

### 1. Display Availability

Shows the number of available parking slots and displays the first 10 available slot numbers.

Example:

```text
Available slots: 100 / 100
Slot numbers: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] ...
```

### 2. Vehicle Entry

The user enters the vehicle number, and the system assigns the first available parking slot.

Example:

```text
Enter choice: 2
Enter vehicle number: ap22idhnr
Vehicle ap22idhnr assigned to slot 1.
```

### 3. Vehicle Exit

The user enters the vehicle number. The system finds the assigned slot, calculates the parking duration, calculates the fee, and releases the slot.

Example:

```text
Enter choice: 3
Enter vehicle number: ap22idhnr
Vehicle ap22idhnr left slot 1.
Duration: 1 hour(s) | Fee: 20 currency units
```

### 4. Exit Program

Selecting option `4` terminates the program.

```text
Enter choice: 4
Exiting system.
```

## Input and Output

### Input

```text
Enter choice: 2
Enter vehicle number: ap22idhnr
```

### Output

```text
Vehicle ap22idhnr assigned to slot 1.
```

When the vehicle exits:

```text
Enter choice: 3
Enter vehicle number: ap22idhnr

Vehicle ap22idhnr left slot 1.
Duration: 1 hour(s) | Fee: 20 currency units
```

## Technologies Used

* **Python 3**
* `datetime` — to record entry and exit times
* `math` — to round parking duration up to the next full hour
* **Dictionary** — to store parking and vehicle information
* **Set** — to manage available parking slots

## Parking Fee Calculation

The system charges:

```text
Fee = Number of Hours × Rate Per Hour
```

The current rate is:

```text
20 currency units per hour
```

For example:

```text
Parking Duration = 2 hours
Rate = 20 per hour

Fee = 2 × 20
Fee = 40 currency units
```

A minimum of **1 hour** is charged for every vehicle.

## Example Flow

```text
--- Parking Management System ---
1. Display Availability
2. Vehicle Entry
3. Vehicle Exit
4. Exit Program

Enter choice: 2
Enter vehicle number: ap22idhnr
Vehicle ap22idhnr assigned to slot 1.

--- Parking Management System ---
1. Display Availability
2. Vehicle Entry
3. Vehicle Exit
4. Exit Program

Enter choice: 3
Enter vehicle number: ap22idhnr
Vehicle ap22idhnr left slot 1.
Duration: 1 hour(s) | Fee: 20 currency units

--- Parking Management System ---
1. Display Availability
2. Vehicle Entry
3. Vehicle Exit
4. Exit Program

Enter choice: 4
Exiting system.
```

## Conclusion

This project demonstrates how **Python dictionaries, sets, functions, loops, date and time handling, and basic calculations** can be combined to create a simple real-world parking management system.
