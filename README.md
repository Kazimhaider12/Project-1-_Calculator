# Project-1-_Calculator
def add(x,y):
    return x+y
def sub(x,y):
    return x-y
def mul(x,y):
    return x*y
def div(x,y):
    return x/y  
def main(): 
    print("\nWelcome to the project Calculator : ")
    print("1.Add ")
    print("2.Subtraction")
    print("3.Multiplication")
    print("4.Divide")
    print("5.Exit")
    print("----- Choice a value to calculate -----")
    while(True):
        choice = int(input("Enter : "))
        if choice == 5:
            print("---- Exit ----")
            break
        if choice in [1,2,3,4] :
                
            x = int(input("Enter 1st Value : "))
            y = int(input("Enter 2nd Value :"))
            
            if choice == 1 :
                print("Addition : " , x , " + ", y , " = ",add(x,y) )
            elif choice == 2:
                print("Subtraction : " , x , " - ", y , " = ",sub(x,y) )
            elif choice == 3:
                print("Multiplication : " , x , " * ", y , " = ",mul(x,y) )
            elif choice == 4:
                print("Divide : " , x , " / ", y , " = ",div(x,y) )
        else:
            print("Enter Invalid input")   

if __name__ == "__main__":
    main()
