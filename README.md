# Filehandling-and-Input
name=str(input("Enter your Name: "))
if name.isdigit():
    print("Error Name will be in Alphabets")
    name=str(input("Enter your Name: "))
colour = str(input("Enter your colour: "))
if colour.isdigit():
    print("Error")
age = int(input("Enter Your age: "))
if age.is_integer() and int(age) < 0:
    print("Error Age must be in positive")
f = open("user_info.txt","w")
f.write(f"Name: {name}\n")
f.write(f"Colour: {colour}\n")
f.write(f"Age: {age}\n")
f.close()


