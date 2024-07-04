# Temperature Warning VI

This VI monitors the current temperature and checks whether it is above the maximum temperature or below the minimum temperature. Based on the condition, it issues a warning in the form of text and an LED indicator.

## Front Panel

1. **Numeric Controls:**
   - `Current Temperature` - Numeric input for the current temperature.
   - `Maximum Temperature` - Numeric input for the maximum threshold temperature.
   - `Minimum Temperature` - Numeric input for the minimum threshold temperature.

2. **Indicators:**
   - `Warning Message` - String indicator to display the warning message.
   - `Heat Stroke LED` - Boolean indicator (LED) that lights up if the temperature is above the maximum threshold.
   - `Freezing Warning LED` - Boolean indicator (LED) that lights up if the temperature is below the minimum threshold.

## Block Diagram

1. Use a comparison operation to check if the current temperature is above the maximum temperature.
2. Use another comparison operation to check if the current temperature is below the minimum temperature.
3. Uses a T/F structure to handle the warning messages and LED indicators based on the comparison results.

## Example

Assume the following values:
- `Current Temperature`: 45
- `Maximum Temperature`: 40
- `Minimum Temperature`: 10

In this case, the VI will display "Heat Stroke Detected" and light up the `LED`.

Here's a pictorial representation:
![Screenshot 2024-07-04 084255](https://github.com/Olowo-samuel/Sam-LabVIEW-Files/assets/107564106/873247c4-9b9c-49f9-8ba9-d0c73901c842)
