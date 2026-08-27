# Parking Management System

## Description

This project contains a Python script that implements a simple **Parking Management System**. It manages **100 parking slots**, assigns available slots to vehicles, and calculates parking fees when vehicles leave.

## How It Works

The program uses functions, dictionaries, and sets to manage the parking area.

The system:

* Displays available parking slots.
* Assigns the first available slot to a vehicle.
* Records the vehicle's entry time.
* Prevents the same vehicle from being parked twice.
* Calculates the parking fee when the vehicle exits.
* Releases the slot after the vehicle leaves.

## Usage

When the script is executed, it displays a menu:


1. Display Availability
2. Vehicle Entry
3. Vehicle Exit
4. Exit Program


The user can select an option and enter the vehicle number when required.

## Input and Output

### Input
Enter choice: 2
Enter vehicle number: ap22idhnr

### Output
Vehicle ap22idhnr assigned to slot 1.

When the vehicle exits:
Vehicle ap22idhnr left slot 1.
Duration: 1 hour(s) | Fee: 20 currency units

