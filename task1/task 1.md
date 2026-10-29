# 1. Problem Statement
Develop a Python program to allocate university scholarships based on students' aggregate marks, subject-wise minimum marks, attendance percentage, and family income. The system identifies eligible students, ranks them according to their aggregate marks, and resolves ties using predefined rules such as higher attendance and lower family income.
# 2. Algorithm
1. Start the program.
2. Read the number of students.
3. Enter each student's name, aggregate marks, subject marks, attendance percentage, and annual family income.
4. Check the eligibility criteria:
   - Aggregate marks ≥ 75%
   - Minimum mark in every subject ≥ 60%
   - Attendance ≥ 75%
   - Annual family income ≤ ₹2,50,000
5. Add eligible students to the scholarship list.
6. Rank students by:
   - Higher aggregate marks first.
   - If marks are equal, higher attendance first.
   - If both are equal, lower family income first.
   - If still tied, alphabetical order of name.
7. Display the eligible students and their ranks.
8. Display a message if no students are eligible.
9. Stop the program.
# 3. Flowchart (Mermaid)
```mermaid

flowchart TD
    A([Start]) --> B[/Enter student details/]
    B --> C{Aggregate >= 75%,\nall subjects >= 60%,\nattendance >= 75%,\nincome <= 250000?}
    C -- Yes --> D[Add to eligible list]
    C -- No --> E[Mark as not eligible]
    D --> F{More students?}
    E --> F
    F -- Yes --> B
    F -- No --> G[Sort eligible students]
    G --> H[Rank by marks, attendance,\nincome and name]
    H --> I[/Display scholarship ranking/]
    I --> J([Stop])
```
# 4. Source Code (Python)

students = []
n = int(input("Enter number of students: "))

for i in range(n):
    print("\nStudent", i + 1)
    name = input("Enter name: ")
    aggregate = float(input("Aggregate marks (%): "))
    subjects = list(map(float, input(
        "Enter 3 subject marks: ").split()))
    attendance = float(input("Attendance (%): "))
    income = float(input("Annual family income (Rs): "))

    if (aggregate >= 75 and min(subjects) >= 60
            and attendance >= 75 and income <= 250000):
        students.append({
            "name": name,
            "marks": aggregate,
            "attendance": attendance,
            "income": income
        })

# Rank by marks, attendance, income, then name
students.sort(key=lambda s: (
    -s["marks"], -s["attendance"],
    s["income"], s["name"].lower()
))

print("\n--- SCHOLARSHIP RESULTS ---")

if students:
    for rank, s in enumerate(students, 1):
        print(f"{rank}. {s['name']} | "
              f"Marks: {s['marks']}% | "
              f"Attendance: {s['attendance']}% | "
              f"Income: Rs.{s['income']:.0f}")
else:
    print("No eligible students found.")
# 6. Sample Output
--- SCHOLARSHIP RESULTS ---
1. Kiran | Marks: 85.0% | Attendance: 95.0% | Income: Rs.200000
2. Ravi | Marks: 85.0% | Attendance: 90.0% | Income: Rs.180000
# 7. Output Screenshot
<img width="598" height="504" alt="image" src="https://github.com/user-attachments/assets/290b47ba-2616-4b0b-9fde-a4f2d6a42260" />
