# -Simple-Data-Filtering-Using-Python

## 1. Project Description

This project demonstrates how to filter student records using Python. Students are filtered based on their marks, age, and department using conditional statements and logical operators.

## 2. Objective

- Create and store student records.
- Filter students based on different conditions.
- Use Python lists, dictionaries, loops, and conditional statements.
- Apply multiple filtering conditions using `and` and `or`.

## 3. Tools Required

- Python 3
- Jupyter Notebook

## 4. Student Dataset and Python Code

### Step 1: Create Student Records

```python
students = [
    {"name": "Ravi", "age": 20, "marks": 85, "department": "CSE"},
    {"name": "Sita", "age": 19, "marks": 92, "department": "ECE"},
    {"name": "Kiran", "age": 21, "marks": 67, "department": "CSE"},
    {"name": "Priya", "age": 20, "marks": 78, "department": "IT"},
    {"name": "Arjun", "age": 22, "marks": 95, "department": "CSE"},
    {"name": "Lakshmi", "age": 18, "marks": 55, "department": "ECE"},
    {"name": "Rahul", "age": 21, "marks": 88, "department": "IT"},
    {"name": "Divya", "age": 19, "marks": 73, "department": "CSE"}
]

print("All Student Records:")
for student in students:
    print(student)
```

### Step 2: Filter Students by Marks

Display students who scored more than 80 marks.

```python
print("Students who scored more than 80 marks:")

for student in students:
    if student["marks"] > 80:
        print(student)
```

### Step 3: Filter Students by Age

Display students younger than 21 years.

```python
print("Students younger than 21:")

for student in students:
    if student["age"] < 21:
        print(student)
```

### Step 4: Filter Students by Department

Display students belonging to the CSE department.

```python
print("Students belonging to the CSE department:")

for student in students:
    if student["department"] == "CSE":
        print(student)
```

### Step 5: Filter Using Multiple Conditions

Display CSE students who scored more than 80 marks.

```python
print("CSE students who scored more than 80 marks:")

for student in students:
    if student["department"] == "CSE" and student["marks"] > 80:
        print(student)
```

Expected students: Ravi and Arjun.

### Step 6: Filter Using the OR Operator

Display students who scored above 90 marks or are younger than 20.

```python
print("Students who scored above 90 OR are younger than 20:")

for student in students:
    if student["marks"] > 90 or student["age"] < 20:
        print(student)
```

### Step 7: Display Results in a Formatted Table

Display students who scored at least 75 marks.

```python
print(f"{'Name':<12} {'Age':<8} {'Marks':<8} {'Department':<12}")
print("-" * 45)

for student in students:
    if student["marks"] >= 75:
        print(
            f"{student['name']:<12} "
            f"{student['age']:<8} "
            f"{student['marks']:<8} "
            f"{student['department']:<12}"
        )
```

## 5. How to Run the Project

1. Install Python 3 on your computer.
2. Install Jupyter Notebook by running:

   ```bash
   pip install notebook
   ```

3. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

4. Create a new Python notebook.
5. Copy each Python code section into a separate cell in the order shown.
6. Run each cell using `Shift + Enter`.
7. Save the notebook as `Simple_Data_Filtering.ipynb`.

## 6. Concepts Used

- Python lists
- Python dictionaries
- For loops
- If statements
- Comparison operators
- Logical operators (`and`, `or`)
- Formatted output

## 7. Expected Output

The program displays student records filtered by marks, age, and department. It also demonstrates filtering with multiple conditions and prints a formatted table of qualifying students.

## 8. Conclusion

This project demonstrates how Python lists, dictionaries, loops, and conditional statements can be used to organize student data and filter records based on specific requirements.

## 9. Project Deliverables

- Student dataset
- Filtering by marks, age, and department
- Multiple-condition filtering
- Display of filtered results
- Jupyter Notebook containing the Python code

