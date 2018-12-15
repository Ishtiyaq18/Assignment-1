# Assignment-1

#1.Install Jupyter notebook and run the first program and share the screenshot of the output.

#Program to identify all divisibles of a number

print('Type a number of your choice')
Number=int(input())
Divisors =[]
denominators=range(1,Number+1)
for N in denominators:
    if Number % N == 0:
        Divisors.append(N)
print(Number,'is divisible by', Divisors)

# 2.Write a program which will find all such numbers which are divisible by 7 but are not a
# multiple of 5, between 2000 and 3200 (both included). The numbers obtained should be printed
# in a comma-separated sequence on a single line.

#We'll start with creating an empty list for getting the required output format
#considering range upto 3201 to include 3200 as part of range
#specifying x as the variable
#defining the criteria
#adding variable within list Y
#adding "," as per requirement in the problem for printing the results

Y=[]
range(2000,3201)
for x in range(2000,3201):
    if (x%7==0 and x%5!=0): 
        Y.append(str(x))
print(','.join(Y)) 

#3. Write a Python program to accept the user's first and last name and then getting them printed
# in the the reverse order with a space between first name and last name.
Firstname= input("Your first name is - ")
Lastname = input("Your last name is - ")
print ('Your name in reverse order is - ',Firstname[::-1],"",Lastname[::-1])

#4. Write a Python program to find the volume of a sphere with diameter 12 cm.
# Formula: V=4/3 * π * r 3

# Program to find the volume of a sphere
#input box for diameter value
Diameter =(int(input('Please type the daimeter of the circle - ')))
#Explanation
print('We know the radius of circle = Daimeter/2')
Radius = Diameter/2
print('So the radius of the circle is - ',Radius)
print('Formula for Volume of circle = 4/3*3.14*Radius*Radius*Radius')
Volume =(4/3*3.14*Radius*Radius*Radius)
#Space before the final result
print('')
#round function used to round of the decimals
print ('Based on the input, the volume of circle is =', (round(Volume,2)),'cm')
