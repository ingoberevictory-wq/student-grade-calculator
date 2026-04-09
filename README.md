# Student Grade Calculator (Advanced Version)

while True:
    name = input("\nEnter student name (or type 'exit' to stop): ")
    
    if name.lower() == "exit":
        print("Program ended.")
        break

    try:
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
        print("Average Score:", round(average, 2))
        print("Grade:", grade)

    except ValueError:
        print("⚠️ Please enter valid numbers!")
