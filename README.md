# Sphere-Calculator
This Python program calculates the Diameter, Circumference, Surface Area, and Volume of a sphere based on a user-provided radius. The program utilizes the mathematical equations associated with these properties to compute accurate results.

Usage
Clone the repository to your local machine:

bash
Copy code
git clone https://github.com/your-username/sphere-calculator.git
Navigate to the project directory:

bash
Copy code
cd sphere-calculator
Run the program:

bash
Copy code
python sphere_calculator.py
Enter the radius of the sphere when prompted.

The program will output the calculated Diameter, Circumference, Surface Area, and Volume rounded to 2 significant digits after the decimal.

Requirements
Python 3.x
math module
fractions module
Code Overview
python
Copy code
# This program is used to find the Diameter, Circumference, Surface Area, and Volume of a sphere using a given radius.
# The radius is user-generated. The radius will be used in certain equations to calculate the correct output.
import math
import fractions

# This is the variable for the fraction in the Volume equation
f1 = fractions.Fraction(4, 3)

# This will be our starting point where we get the radius input from the user.
# It will get a float value since it has a decimal.
radius = float(input("What is the radius of a sphere: "))

# This is where all the math will be complete and rounded to 2 significant digits after the decimal
diameter = round(2 * radius, 2)
circumference = round(diameter * math.pi, 2)
Surface_Area = round(4 * math.pi * radius * radius, 2)
Volume = round(f1 * math.pi * radius * radius * radius, 2)

# Output after the equations are complete
print("Diameter:", diameter)
print("Circumference:", circumference)
print("Surface Area:", Surface_Area)
print("Volume:", Volume)
Contributing
Feel free to contribute to the project by submitting pull requests or reporting issues.

License
This project is licensed under the MIT License - see the LICENSE file for details.
