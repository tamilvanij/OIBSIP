def calculate_bmi(weight, height):
    return weight / (height ** 2)

def classify_bmi(bmi):
    if bmi < 18.5:
        return "Underweight"
    elif bmi < 25:
        return "Normal"
    elif bmi < 30:
        return "Overweight"
    else:
        return "Obese"

while True:
    try:
        weight = float(input("Enter weight in kg: "))
        height = float(input("Enter height in meters: "))
        if weight <= 0 or height <= 0:
            print("Weight and height must be positive numbers.")
            continue
        bmi = calculate_bmi(weight, height)
        category = classify_bmi(bmi)
        print(f"Your BMI is: {bmi:.2f}")
        print(f"Category: {category}")
    except ValueError:
        print("Please enter valid numbers for weight and height.")

    again = input("Do you want to calculate BMI for another person? (yes/no): ").strip().lower()
    if again != "yes":
        print("Thank you for using the BMI calculator!")
        break
