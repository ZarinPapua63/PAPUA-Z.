Here is the updated documentation specifically tailored for Python:

**Project Title**

2D Distance Calculator

**Description**

A console application written in Python that calculates the straight-line distance between two points on a 2D Cartesian plane using the distance formula:

$$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$

### How to Run the Program

1. Save the code in a file named `distance_calculator.py`.
2. Open your terminal or command prompt and navigate to the folder containing the file.
3. Execute the script:
```bash
python distance_calculator.py

```



### Input Needed

The program requires four numerical inputs:

* $x_1$: X-coordinate of the first point
* $y_1$: Y-coordinate of the first point
* $x_2$: X-coordinate of the second point
* $y_2$: Y-coordinate of the second point

### Sample Output

```text
=== 2D Distance Calculator (Python) ===
Enter x1: 3
Enter y1: 4
Enter x2: 7
Enter y2: 1

Calculating distance...
The distance between (3.0, 4.0) and (7.0, 1.0) is 5.00 units.

```

### Author

Created by [Zarin Papua]

---

### Python Code Implementation

Here is the source code if you need it:

```python
import math

def calculate_distance():
    print("=== 2D Distance Calculator (Python) ===")
    try:
        x1 = float(input("Enter x1: "))
        y1 = float(input("Enter y1: "))
        x2 = float(input("Enter x2: "))
        y2 = float(input("Enter y2: "))
        
        distance = math.sqrt((x2 - x1)**2 + (y2 - y1)**2)
        print(f"\nThe distance between ({x1}, {y1}) and ({x2}, {y2}) is {distance:.2f} units.")
    except ValueError:
        print("Invalid input. Please enter numbers only.")

if __name__ == "__main__":
    calculate_distance()

```
