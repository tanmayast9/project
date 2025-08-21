# project
simple bank system using python
name=input("Enter your name: ")
print("Welcome to the bank system, " + name + "!")

acc_no=int(input("Enter your account number: "))
balance=0
print("Your account number is: " + str(acc_no))

while True:
    print("choose an option")
    print("1.withdraw amount")
    print("2.deposit amount")
    print("3.check balance")
    print("4.exit")

    choice = int(input("enter choice(1-4)"))

    if choice==1 :
        debt=int(input("enter amount to withdraw "))
        if debt>balance :
            print("insufficient balance")
        else :
            balance-=debt
            print("your balance is ",balance)

    elif choice==2 :
        credit=int(input("enter amount to deposit"))
        balance+=credit
        print("the amount credited is",balance)

    elif choice==3 :
        print("your balance is",balance)

    elif choice==4:
        print("thank you for chosing us, goodbye!")
        break

    else:
        print("invalid choice try again")
