# Hackerrank
## Solutions to introductionary problems in Python 3

### Python If-Else

Prints out 'Weird' if the number is odd and between the range of 6 and 21, otherwise 'Not Weird'.
```
n = int(input("Write a digit: "))
if(n % 2 != 0 or n in range(6, 21)):
    print("Weird")
else:
    print("Not Weird")
```

### Arithmetic Operatotrs

Performs arithmetic calcutions with +,-, *
```
print("Write a and b numbers to perfom arithmetic calculations:")
a = int(input("a: "))
b = int(input("b: "))
print("{:d}\n{:d}\n{:d}".format(a+b,a-b,a*b))
```

### Python Division

Performs divisions
```
print("Write a and b numbers to perfom division calculations:")
a = int(input("a: "))
b = int(input("b: "))
print("{:d}\n{:f}".format(a//b,a/b))
```

### Loop

Will loop through n numbers starting from 0 and perfrom power on each and print them out
```
n = int(input("Write a number: "))
for i in range(n):
    print(i**2)
```

### Write A Function

Finds out if the year is leap year or not
```
def is_leap(year):
    leap = False
    
    
    if(year % 400 == 0):
        leap = True
    elif(year % 4 == 0 and year % 100 !=0):
        leap = True
    return leap

print(is_leap(int(input("Write a year to find out if its a leap year: "))))
```

### Print Function

Prints numbers from 0 to n
```
def is_leap(year):
    leap = False
    
    
    if(year % 400 == 0):
        leap = True
    elif(year % 4 == 0 and year % 100 !=0):
        leap = True
    return leap

print(is_leap(int(input("Write a year to find out if its a leap year: "))))
```

### Sorting: Bubble Sort

Counts how many times bubble sort will perform sorting
```
def countSwaps(a):
    counter = 0
    not_sorted = True
    while not_sorted:
        not_sorted = False
        for i in range(len(a)-1):
          if a[i] > a[i+1]:
            a[i], a[i+1] = a[i+1], a[i]
            counter +=1
            not_sorted = True
    print("Array is sorted in {} swaps.".format(counter))
    print("First Element: {}".format(a[0]))
    print("Last Element: {}".format(a[-1]))

print(countSwaps([4,3,2,1]))
```
