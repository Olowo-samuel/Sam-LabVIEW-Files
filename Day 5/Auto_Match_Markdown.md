# Auto Match VI Explanation

## Overview

I have created and implemented a Virtual Instrument (VI) that implements the WHILE loop to perform a particular task: it continuously generates random numbers between 0 and 1000 until it generates a number that matches a number selected by the user.

## Functionality

1. **User Input**: The user selects a target number within the range of 0 to 1000. A limit has been established using unsigned integers. If the user enters a number outside the range of 0 to 1000, the control adjusts it to the nearest valid value within that range. 
2. **Random Number Generation**: The VI begins generating random numbers within the same range.
3. **Matching Process**: The generation continues until the VI produces a random number that matches the user's selected number.
4. **Count Determination**: The VI also tracks and determines the number of random numbers generated before achieving the match.

## Usage

- **Step 1**: The user inputs their selected number (let's call it `known_number`).
- **Step 2**: The VI starts generating random numbers.
- **Step 3**: The VI compares each generated number with the `known_number`.
- **Step 4**: Once the generated number equals the `known_number`, the VI stops.
- **Step 5**: The VI outputs the count of the random numbers generated during the process.

## Example

For instance, if the user selects `50` as the known number:

- The VI begins generating random numbers between 0 and 1000.
- If the VI generates numbers like 123, 789, 456, ..., and eventually 50, it will stop.
- The VI then shows how many numbers were generated before matching 50.

## Visual Representation
![Screenshot 2024-06-21 002414](https://github.com/Olowo-samuel/Sam-LabVIEW-Files/assets/107564106/2b278f62-cccc-4344-a03a-28ab31c9546b)

Feel free to reach out if you have any questions or need further details about this VI!
