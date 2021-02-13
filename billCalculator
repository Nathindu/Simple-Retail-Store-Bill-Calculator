# print topic which gives as a parameter
def topic_print(topic):
    print()
    print()
    for x in range(25):
        print("-", end=" ")
    print(topic, end=" ")
    for x in range(25):
        print("-", end=" ")


# calculates the discount according to price
def calculate_discount(price):
    discount = 0
    if price > 5000:
        discount = price * 0.1

    elif price > 15000:
        discount = price * 0.2

    elif price > 5000:
        discount = price * 0.35

    return discount


# check a valid item or not
# hard coded item list
def check_item(item):
    valid = False
    if item == "sr23":
        valid = True

    elif item == "sr45":
        valid = True

    elif item == "sr48":
        valid = True

    elif item == "sr41":
        valid = True

    elif item == "sr62":
        valid = True

    elif item == "sr20":
        valid = True

    return valid


# returns the item price
# hard coded item list with price
def item_price(item):
    value = 0
    if item == "sr23":
        value = 2500.00

    elif item == "sr45":
        value = 3490.00

    elif item == "sr48":
        value = 4790.00

    elif item == "sr41":
        value = 2390.00

    elif item == "sr62":
        value = 2500.00

    elif item == "sr20":
        value = 1200.00

    return value


# calculates the total with discount
def calculate_total(total):
    print()
    print("TOTAL: ", end="")
    print(total)

    print("DISCOUNT: ", end="")
    print(calculate_discount(total))  # calling thr discount method

    print("AMOUNT TO PAY: ", end="")
    print(total - calculate_discount(total))  # total - discount


topic_print("WELCOME TO TEXTILE SHOP BILL CALCULATOR")
print()
print()

print("TO CALCULATE ENTER THE ITEM NUMBERS AND AMOUNT OR ENTER 'C' TO CALCULATE THE BILL")

totalAmount = 0
while True:
    print()
    itemNo = input("ENTER THE ITEM NO OR TO CALCULATE THE BILL ENTER 'C': ")
    itemNo = itemNo.replace(" ", "")
    itemNo = itemNo.lower()

    if itemNo == "c":  # calculates the bill
        calculate_total(totalAmount)
        topic_print("THANK YOU FOR SHOPPING WITH US ")
        break

    elif check_item(itemNo):  # checks the item availability and takes the input
        itemQty = int(input("ENTER THE QUANTITY: "))
        totalAmount += itemQty * item_price(itemNo)

    else:
        print("INVALID ITEM CODE")
