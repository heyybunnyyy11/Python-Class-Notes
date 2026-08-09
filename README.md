# Python Day 3 - ATM Machine

balance = 10000
pin = 1234

entered_pin = 1234
choice = 3
withdraw_amount = 2500

print("===== WELCOME TO ATM =====")

if entered_pin == pin:

    print("PIN Correct!")
    print("\n1. Check Balance")
    print("2. Deposit Money")
    print("3. Withdraw Money")

    print("\nSelected Option:", choice)

    if choice == 1:
        print("Your Balance is:", balance)

    elif choice == 2:
        deposit_amount = 3000
        balance = balance + deposit_amount

        print("Deposited Amount:", deposit_amount)
        print("New Balance:", balance)

    elif choice == 3:

        if withdraw_amount <= balance:
            balance = balance - withdraw_amount

            print("Withdrawal Amount:", withdraw_amount)
            print("Please Collect Your Cash")
            print("Remaining Balance:", balance)

        else:
            print("Insufficient Balance")

    else:
        print("Invalid Choice")

else:
    print("Wrong PIN")

Output:

===== WELCOME TO ATM =====
PIN Correct!

1. Check Balance
2. Deposit Money
3. Withdraw Money

Selected Option: 3
Withdrawal Amount: 2500
Please Collect Your Cash
Remaining Balance: 7500