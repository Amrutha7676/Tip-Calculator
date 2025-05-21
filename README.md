# Tip-Calculator
def tip_calculator():
    print("Welcome to the Tip Calculator!")
    
    bill = float(input("Enter the bill amount: $"))
    tip_percent = float(input("Enter tip percentage (e.g., 10, 15, 20): "))
    people = int(input("Split between how many people? "))

    tip_amount = bill * (tip_percent / 100)
    total_bill = bill + tip_amount
    amount_per_person = total_bill / people

    print(f"\nTotal Tip: ${tip_amount:.2f}")
    print(f"Total Bill (with Tip): ${total_bill:.2f}")
    print(f"Each person should pay: ${amount_per_person:.2f}")

tip_calculator()
