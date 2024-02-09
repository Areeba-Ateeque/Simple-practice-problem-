# Simple-practice-problem-
#1.
unit_price = int(input("Enter the unit price: "))
quantity = int(input("Enter the quantity: "))
total_cost = unit_price * quantity

# Applying a 10% discount if the total cost exceeds $1000
if total_cost > 1000:
    discount = 0.1 * total_cost
    total_cost -= discount

# Displaying the total cost
print(f"The total cost is: ${total_cost:.2f}")
#2
temperature_celsius = int(input("Enter the current temperature in Celsius: "))
# Checking if the temperature is below 20°C and advising on wearing a jacket
if temperature_celsius < 20:
    print("It's recommended to wear a jacket.")
else:
    print("No need for a jacket.")
#3.
side1 = int(input("Enter the length of the first side: "))
side2 = int(input("Enter the length of the second side: "))
side3 = int (input("Enter the length of the third side: "))
if side1 == side2 == side3:
    print("Equilateral Triangle")
elif side1 == side2 or side1 == side3 or side2 == side3:
     print("Isosceles Triangle")
else:
    print("Scalene Triangle")
#4.  
pin = input("Enter your PIN: ")

if pin == "5678":
    withdrawal_amount = int(input("Enter the amount you want to withdraw: "))
    balance = 1000  # Assuming the initial balance is 5000

    if withdrawal_amount <= balance:
        balance -= withdrawal_amount
        print("Withdrawal successful")
    else:
        print("Insufficient balance.")
else:
    print("Invalid PIN.")
#5.
score=int(input("Enter a scores: "))
if 90 <= score <= 100:
       print("A")
elif 80 <= score < 90:
        print("B")
elif 70 <= score < 80:
       print( "C")
elif 60 <= score < 70:
        print("D")
else:
        print("F")

# 6.
user_input = input("Enter a month (as a number): ")
month_number = int(user_input)
days_in_month = {
    1: 31,  # January
    2: 28,  # February (considering a non-leap year)
    3: 31,  # March
    4: 30,  # April
    5: 31,  # May
    6: 30,  # June
    7: 31,  # July
    8: 31,  # August
    9: 30,  # September
    10: 31, # October
    11: 30, # November
    12: 31  # December
}
    # Check if the input month is valid
if 1 <= month_number <= 12:
    print(f"Number of days in month {month_number}: {days_in_month[month_number]}")
else:
    print("Invalid month input. Please enter a number between 1 and 12.")
