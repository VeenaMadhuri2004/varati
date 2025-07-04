def hrec(n):
if n==0:
            return
            hrec(n-1)
            print(n)
num=int(input("enter the value:")
hrec(num)

#linear recursion factorial
def fact(n):
    if n==1:
        return 1
    return n*fact(n-1)
num=int(input("enter a number:"))
print("factorial:",fact(num))

def sumD(n):
    if n==0:
        return 0
    return (n%10)+sumD(n//10)
num=int(input("enter n:"))
print(sumD(num))

#indirect rec
def one(n):
    if n>0:
        print("one:", n)
        two(n-1)
def two(n):
    if n>0:
        print("two:", n)
        one(n//2)
num=int(input("enter the value of n:"))
one(num)

def is_even(n):
    if n==0:
        return True
    return is_odd(n-1)
def is_odd(n):
    if n==0:
        return False
    return is_even(n-1)
num=int(input("enter any number:"))
print(num,"is even?",is_even(num))

def tree(n):
    if n<0:
        return
    print(n)
    tree(n-1)
    tree(n-2)
tree(3)


def nest(n):
    if n>=10:
        return n-1
    return(nest(nest(n+2)))
print(nest(5))
