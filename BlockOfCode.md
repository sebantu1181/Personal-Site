# **This is My Block of Code!**

_Write a Python 3 program called **cylindervolumecalc.py** that accepts user input from the keyboard for the radius and height of the cylinder and outputs the volume based on the equation for the volume of a cylinder provided in the requirements._

#### _This is my code from IT-1040_
```python
#This program is going to calculate the Volume of a Cylinder
#Volume = pi * r^2 * h

import math

def calculate_volume(radius,height):
     volume = math.pi * radius ** 2 * height
     return volume

def get_radius_from_user():
     while True:
          try:
               radius = float(input("Enter the radius: "))
               if radius < 0:
                    print("The radius must be  0 or greater")
                    continue
               break
          except Exception as e:
               print(e)
               
     return radius

def get_height_from_user():
     while True:
          try:
               height = float(input("Enter the height: "))
               if height < 0:
                    print("The height must be 0 or greater")
                    continue
               break
          except Exception as e:
               print(e)
               
     return height

def generate_report(radius,height,volume):
    print("Radius of the cylinder is",radius, "square times the height",height, "equals the volume of", volume)

def main():
    radius = get_radius_from_user()
    height = get_height_from_user()
    volume = calculate_volume(radius,height)
    generate_report(radius,height,volume)

main()

```

[Link to Mizzou Survey](MizzouSurvey.md)
