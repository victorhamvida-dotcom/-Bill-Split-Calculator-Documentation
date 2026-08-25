# 🧾-Bill-Split-Calculator-Documentation
This project implements a simple Python-based calculator to split a bill among multiple people, including tip calculation. It demonstrates basic programming concepts such as user input handling, arithmetic operations, and formatted output.
 
### Table of Contents
-	Executive Summary
-	Business Problem
-	Dataset / Inputs Overview
-	Code Workflow (Data Cleaning Equivalent)
-	Feature Engineering (Derived Values)
-	Output / KPI Dashboard
-	Business Insights
-	Technical Skills Demonstrated
-	Project Outcome

## 1. Executive Summary
This project implements a simple Python-based calculator to split a bill among multiple people, including tip calculation. It demonstrates basic programming concepts such as user input handling, arithmetic operations, and formatted output.

The calculator computes:
-	Tip amount based on user-specified percentage
-	Total bill including tip
-	Equal share per person

This tool is useful for quick expense sharing in group dining or social settings.

## 2. Business Problem
When dining out or sharing expenses, calculating each person’s contribution can be error-prone and time-consuming. Manual calculations often lead to confusion, especially when tips are included.

The purpose of this project is to automate the process, ensuring accuracy and fairness in bill splitting.

## 3. Dataset / Inputs Overview
this project relies on user inputs rather than external data files.
| Input Variable   | Description                     | Example |
|------------------|---------------------------------|---------|
| bill_amount      | Total bill before tip           | 100.00  |
| tip_percentage   | Tip percentage to apply         | 10      |
| num_people       | Number of people sharing the bill | 4     |


## 4. Code Workflow (Data Cleaning Equivalent)
Steps performed by the program:
1.	Accepts user inputs for bill, tip, and number of people.
2.	Converts inputs into numeric values (float or int).
3.	Calculates tip amount.
4.	Adds tip to bill to get total.
5.	Divides total by number of people.
6.	Prints results in a clear format.
5. Feature Engineering (Derived Values)

The program generates new values from raw inputs:
| Feature             | Formula                                | Purpose                   |
|---------------------|----------------------------------------|---------------------------|
| tip_amount          | (tip_percentage / 100) * bill_amount   | Shows tip contribution    |
| total_amount        | bill_amount + tip_amount               | Total bill including tip  |
| amount_per_person   | total_amount / num_people              | Fair share per person     |


## 7. Output / KPI Dashboard
The calculator produces two key outputs:
- Total (including tip): e.g., $110.0
- Each person pays: e.g., $27.5

These outputs act as the KPIs of the program, ensuring clarity and fairness.

## 8. Business Insights
-	Automates bill splitting, reducing manual errors.
-	Ensures fairness by dividing equally among participants.
-	Flexible for different tip percentages and group sizes.
  
### 9. Technical Skills Demonstrated
-	Python programming basics
-	Input handling (input())
-	Type conversion (float, int)
-	Arithmetic operations
-	String formatting with f-strings

## 10. Project Outcome
The project successfully provides a simple, reliable tool for splitting bills. It demonstrates how Python can be applied to everyday problems, reinforcing programming fundamentals while delivering practical value.

 Code
```
print("Bill Split Calculator")
bill_amount = float(input())
tip_percentage = float(input())
tip_amount = (tip_percentage/100)*bill_amount
total_amount = tip_amount + bill_amount


num_people = int(input())
amount_per_person = total_amount /num_people


print(f"Total (including tip): ${total_amount}")
print(f"Each person pays: ${amount_per_person}")

```
