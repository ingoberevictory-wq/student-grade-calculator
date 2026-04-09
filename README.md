# Student Grade Calculator

name = input("Enter student name: ")
score1 = float(input("Enter first score: "))
score2 = float(input("Enter second score: "))
score3 = float(input("Enter third score: "))

average = (score1 + score2 + score3) / 3

if average >= 70:
    grade = "A"
elif average >= 60:
    grade = "B"
elif average >= 50:
    grade = "C"
else:
    grade = "F"

print("\nStudent:", name)
print("Average Score:", average)
print("Grade:", grade)
