```python
#Stack_Implementation_In_Python
```


```python
stack = []
length = int(input("Enter the maximum length of the stack:"))
n = True
while (True):
    print("Choose the operation you want to perform :")
    print("1.push()\n2.pop()\n3.display()\n4.size()\n5.exit()")
    user_input=0
    while(user_input>=0 and user_input<=5):
        user_input = int(input("Choose the operation : "))


        if user_input == 1:
            if len(stack) > length-1:
                    print("OVERFLOW")
            else:
                    element = int(input("Enter the element you want to add in a stack: "))
                    stack.append(element)



        elif user_input == 2:
            if len(stack) <= 0:
                    print("UNDERFLOW")
            else:
                    stack.pop()



        elif user_input == 3:
            print(stack)



        elif user_input == 4:
            print(len(stack))



        elif user_input == 5:
            n = False
            break

        else:
            print("Invalid Syntax.Please Try Again!")

#contributed by Randrita Sarkar



```

    Enter the maximum length of the stack:3
    Choose the operation you want to perform :
    1.push()
    2.pop()
    3.display()
    4.size()
    5.exit()
    Choose the operation : 1
    Enter the element you want to add in a stack: 10
    Choose the operation : 1
    Enter the element you want to add in a stack: 20
    Choose the operation : 1
    Enter the element you want to add in a stack: 30
    Choose the operation : 1
    OVERFLOW
    Choose the operation : 3
    [10, 20, 30]
    Choose the operation : 4
    3
    Choose the operation : 2
    Choose the operation : 3
    [10, 20]
    Choose the operation : 2
    Choose the operation : 2
    Choose the operation : 2
    UNDERFLOW
    Choose the operation : 5
    Choose the operation you want to perform :
    1.push()
    2.pop()
    3.display()
    4.size()
    5.exit()
    


```python

```
