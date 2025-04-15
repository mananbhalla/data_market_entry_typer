
# data_market_entry_typer
# data_market_entry_typera1 = "123456789DCSNMCDMBFM"
a = "true"
print(a)

if a == "true":
    b = input("Do you want to continue to the data inventory system for the marketing system? (y/n): ").lower()
    match b:
        case "y":
            print("You chose to continue.")
            c = input("Do you want to go further to enter your details to create your inventory system? (y/n): ").lower()
            match c:
                case "y":
                    d = int(input("Enter the number of items you want to enter in the inventory system: "))
                    for _ in range(d):
                        k = int(input("Enter the number of digits for the codes or prices: "))
                        if k <= 0:
                            print("The number you entered is invalid. Please enter a positive number.")
                        else:
                            e = input("Enter the item name: ")
                            f = input("Enter the item code: ")
                            g = input("Enter the item price: ")
                            h = input("Enter the item quantity: ")
                            i = input("Enter the item description: ")
                            j = [e, f, g, h, i]
                            print("The number of items entered by you is:", len(j))
                            print("The data entered by you is:", j)
                case "n":
                    print("You chose not to proceed further. Exiting the program.")
                case _:
                    print("Invalid input. Please enter 'y' or 'n'.")
        case "n":
            print("You chose not to continue. Exiting the program.")
        case _:
            print("Invalid input. Please enter 'y' or 'n'.")
else:
    print("The program is not set to 'true'. Exiting.")



