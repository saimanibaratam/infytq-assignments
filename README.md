# infytq-assignments

in this editing window is not clear plz go throw up file

import calendar


def loop_year(year, number_of_years):
    leap_year_counter = 0
    while leap_year_counter < number_of_years:
        if calendar.isleap(year):
            print('{} is a leap year!'.format(year))
            leap_year_counter += 1
        year += 1
loop_year(2016, 15)





next 15 leap years :-



year = int(input("Input a year: "))

if (year % 400 == 0):
    leap_year = True
elif (year % 100 == 0):
    leap_year = False
elif (year % 4 == 0):
    leap_year = True
else:
    leap_year = False

month = int(input("Input a month [1-12]: "))

if month in (1, 3, 5, 7, 8, 10, 12):
    month_length = 31
elif month == 2:
    if leap_year:
        month_length = 29
    else:
        month_length = 28
else:
    month_length = 30


day = int(input("Input a day [1-31]: "))

if day < month_length:
    day += 1
else:
    day = 1
    if month == 12:
        month = 1
        year += 1
    else:
        month += 1
print("The next date is [yyyy-mm-dd] %d-%d-%d." % (year, month, day))
















18/6
numbers:- 

def find_max(num1, num2):

    max_num=-1
    num_list=[] 
    if(num1<num2): 
        for numbers in range(int(num1),int(num2)+1): 
            tot=0
            count=0
            while(numbers>0): 
                digit=numbers%10
                tot=tot+digit 
                numbers=numbers//10 
                count=count+1
                    num_list.append(numbers) 
                else:
                    print(-1)
    else:
        print(-1)
    max_num = max(num_list) #to find the maximum value in the list
    return max_num

#Provide different values for num1 and num2 and test your program.
max_num=find_max(10,15)
print(max_num)





chicken:-

h=int(input())
l=int(input())
p=l/h
c=p-2
r=4-p
if(r==0):
    print(0,1//h)
    elif c==0:
        print(1//h,0)
        else:
            k=c\r
            chicken=round((1*(k)//2))
            rab=round(1*(k)/4)



pattern:-

print("Program to print half pyramid: ")
rows = input("Enter number of rows ")
rows = int (rows)
for i in range (rows,0,-1):
    for j in range(0, i,1):
        print("*", end=' ')
    print("\r")




triangle:-

def form_triangle(num1,num2,num3):
    #Do not change the messages provided below
    success="Triangle can be formed"
    failure="Triangle can't be formed"

    #Write your logic here
    if (num1 + num2 <= num3) or (num1 + num3 <= num2) or (num2 + num3 <= num1) : 
        return failure
    else: 
        return success     
#Provide different values for the variables, num1, num2, num3 and test your program
num1=3
num2=3
num3=5

if form_triangle(num1,num2,num3):
    print("Valid")  
else: 
    print("Invalid") 





