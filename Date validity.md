day   = int(input("enter the day"))
month = int(input("enter the month"))
year  = int(input("enter the year"))

if day < 1 or day > 31 or month < 1 or month > 12 or year < 1 or year > 2020 :
        print ("The date is not valid ")
elif month == 4 or month == 6 or month == 9 or month == 11 :
        if day > 30 :
            print("The date is not valid ")
        if year == 2020 and month == 11 :
            if day > 1 :
                print("The date is not valid ")
            else :
                print("The date is valid ")
elif month == 2 :
        if year % 4 != 0 :
            if day > 28 :
                print("The date is not valid ")
            else :
                print("The date is valid ")
        else:
             print("The date is valid ")
elif month == 12 and year == 2020 :
         print("The date is not valid ")
else :
        print("The date is valid ")
