
## Code Block
This code is from earlier this year and it calculate the volume of a cylinder.
import math

areaperpint = 400/8

while(True):
    radius = float(input("Enter radius of cylinder : "))
    height = float(input("Enter height of cylinder : "))
    costperpint = float(input("Enter cost per pint : "))
    
    if (radius < 0 or height < 0 or costperpint < 0):
        print("Invalid Input")
        continue
    
    area = (2 * math.pi * radius) * (height + radius)
    totalpints = math.ceil(area/areaperpint)
    totalcost =totalpints * costperpint
    
    print("Total Cost :$", round(totalcost,2))
    print("Total Pints :", totalpints)
    
    morecalc = input("Do you want another calculation (Y/N): ")
    
    if morecalc.upper() == 'Y':
        continue
    else:
        break
    




*[Home Page](./README.md)
