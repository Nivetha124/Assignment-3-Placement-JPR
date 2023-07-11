# Assignment-3-Placement-JPR
# 1) Get three number a,b,c. Print 1 if the three numbers are in strictly increasing order (a>b>c)
# Print 2 if the three numbers are decreasing order (a<b<c) otherwise print 0.

def greatestnumber(A,B,C):
    if (A<B) and (B<C):
        return 1
    elif(A>B) and (B>C):
        return 2
    else:
        return 0

A=int(input())
B=int(input())
C=int(input())
print(greatestnumber(A,B,C))

                             (OR)
A=int(input("enter the first number"))
B=int(input("enter the second number"))
C=int(input("enter the third number"))
if (A<B) and (B<C):
    print(1)
elif(A>B) and (B>C):
    print(2)
else:
    print(0)
    
# 2) X + Y = Z Input: 22 50 , Output: 22 , 28 , 50
x=int(input())
z=int(input())
y=z-x
print(x, y, z)

# 3) You are given N numbers {X1,X2,…XN} and Z . Print N pairs X1 , Y1 such that X1 + Y1 = Z
Input : 4 12 25 55 34 100
output :12 , 88
        25 , 75
        55 , 45
        34 , 66
x=list(map(int,input().split()))
z=int(input())
for i in x:
    y=z-i
    print(i,",",y)

# 4) prime number or not
x=int(input())
if x>1:
    for i in range(2,int(x/2)+1):
        if x%i==0:
             print(x,"is not a prime number")
             break
        else:
            print(x,"is a prime number")
            break
else:
    print(x,"is not a prime number")
                                 (OR)

def is_prime_trial_division(n):
    # Check if the number is less than
    # or equal to 1, return False if it is
    if n <= 1:
        return False
    # Loop through all numbers from 2 to
    # the square root of n (rounded down to the nearest integer)
    for i in range(2, int(n ** 0.5) + 1):
        # If n is divisible by any of these numbers, return False
        if n % i == 0:
            return False
    # If n is not divisible by any of these numbers, return True
    return True
  #Test the function with n = 11
  print(is_prime_trial_division(11))

# 5)Find the sum of the digits of the given number Input : 4352 Output : 14
 m=input()
 sum=0
 for i in m:
     sum=sum +int(i)
 print(sum)
                                                     (OR)
num = int(input())
sum = 0

while num!=0:
	digit = int(num)%10
	sum += digit
	num = num/10
print(sum)

# 6) Reverse the number
num = 123456
print(str(num)[::-1])
                                                      (OR)
num=int(input())
reverse_no=0
while num!=0:
    digit=num%10
    reverse_no=reverse_no*10+digit
    num=num//10
print(reverse_no)

# 7)Palindrome or not
num = 1224
temp = num
reverse = 0
while temp > 0:
    remainder = temp % 10
    reverse = (reverse * 10) + remainder
    temp = temp // 10
if num == reverse:
  print('Palindrome')
else:
  print("Not Palindrome")
                                                            (OR)
num = 1234
reverse = int(str(num)[::-1])
if num == reverse:
  print('Palindrome')
else:
  print("Not Palindrome")



                                





















