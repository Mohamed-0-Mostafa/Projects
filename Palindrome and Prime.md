def is_palindrome():
    word = input("Enter the word you want to check: ")
    if word == word[::-1] :
        print("Yes")
    elif word != word[::-1] :
        print("No")
    show_menu()
def is_prime(num):
        if num < 2 :
            print(num, " is not a prime number")
        elif num == 2 :
            print(num, " is a prime number")
        else :
            for i in range(2, num):
                if (num % i == 0) :
                    print(num , " is not a prime number")
                    break
                else :
                    print(num, " is a prime number")
                    break
        show_menu()
def show_menu():
    print()
    print("Choose an operation")
    print("[1] Check Palindrome")
    print("[2] Check if Prime")
    print("[00] Exit")
    operation = int(input())
    if operation == 1 :
        is_palindrome()
    elif operation == 2 :
        num = int(input("Enter the number: "))
        is_prime(num)
    elif operation == 00 :
        print("Thanks for using this program")
    else :
        print("Invalid choice, Please try again")
        show_menu()


show_menu()
