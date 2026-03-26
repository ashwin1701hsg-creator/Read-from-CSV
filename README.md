# Read-from-CSV

## AIM:

## ALGORITHM:
### Step 1:Start the program.
### Step 2: Import the required module (csv or pandas).
### Step 3:Open the CSV file in read mode.
### Step 4:Read the data from the CSV file.
### Step 5:Display the contents of the CSV file.


## PROGRAM:
```
import csv
import os

filename = "data.csv"
if not os.path.exists(filename):
    with open(filename, "w", newline="") as f:
        writer = csv.writer(f)
        writer.writerow(["Name", "Age", "City"])
        writer.writerow(["Alice", 25, "New York"])
        writer.writerow(["Bob", 30, "Los Angeles"])
        writer.writerow(["Charlie", 22, "Chicago"])
    print("Sample CSV created.")
with open(filename, "r") as f:
    reader = csv.reader(f)
    print("\nContents of CSV:")
    for row in reader:
        print(row)
```
## OUTPUT:
<img width="916" height="160" alt="image" src="https://github.com/user-attachments/assets/84dfa0ea-4dfd-4120-8045-6a53e9036723" />

## RESULT:
