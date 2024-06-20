# Understanding Shift Registers in Our Virtual Instruments

In this Virtual Instrument (VI), we make use of shift registers to maintain state information between iterations of a loop. Specifically, we use two shift registers: **top iteration** and **previous iteration**. Here's a brief overview of how this works:

## Initial Setup

1. **Initialized Shift Register**: The shift register is initialized with the constant value **0**. This is our starting point.

## Iterative Process

2. **Iteration and Increment**: On each iteration of the loop, the current value of the shift register is incremented by 1.
3. **Number of Iterations**: This process is repeated for a total of **5 iterations**.

## Summary of the Process
- **Initial Value** = 0
- **Iteration 1**: Starts with the initial value of 0. After the first iteration, the value becomes 1.
- **Iteration 2**: Takes the value from the previous iteration (1) and increments it by 1, resulting in 2.
- **Iteration 3**: The value from the previous iteration (2) is incremented to 3.
- **Iteration 4**: The value from the previous iteration (3) is incremented to 4.
- **Iteration 5**: The value from the previous iteration (4) is incremented to 5.

By the end of the 5th iteration, the first shift register(top iteration) will hold the value **4** and the second shift resgister(previous iteration) will hold the value **3**.

## Visual Representation

Here is a simplified representation of the process:

![Screenshot 2024-06-20 235927](https://github.com/Olowo-samuel/Sam-LabVIEW-Files/assets/107564106/2785c645-e0d0-4bb2-94ee-d026ad4f170a)
