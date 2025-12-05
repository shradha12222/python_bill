# python_bill
print("Welcome to Python's Online Pizza Delivery!")
 size = input("Which size of pizza would you like? S, M, or L: ").upper()
 seasoning = input("Would you like seasoning? Y or N: ").upper()
 extra_cheese = input("Would you like extra cheese? Y or N: ").upper()
 bill = 0
 if size =="S":
     bill += 60
 elif size == "M":
    bill +=80
 else:
   bill +=100

 if seasoning == "Y":
     if size == "S":
       bill += 10
     elif size == "M":
       bill += 15
    else:
      bill +=20

 if extra_cheese == "Y":
     bill += 30

 message = f"You have ordered {size} size Pizza with seasoning= {seasoning} and extra cheese= {extra_cheese} Your Bill =₹ {bill}"
 print("\n")
 print(message)
