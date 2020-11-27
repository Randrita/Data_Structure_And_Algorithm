```python
#Queue_Implementation_In_Python
```


```python
queue = []
length = int(input("Enter the maximum length of the queue:"))
n = True
while (True):
    print("Choose the operation you want to perform :")
    print("1.enqueue()\n2.dequeue()\n3.display()\n4.exit()")
    user_input=0
    while(user_input>=0 and user_input<=5):
        user_input = int(input("Choose the operation : "))


        if user_input == 4:
            print("Operation Exist")
        elif user_input == 1:
            if len(queue) > length-1:
                    print("OVERFLOW")
            else:
                    element = int(input("Enter the element you want to add in a queue: "))
                    queue.append(element)



        elif user_input == 2:
            if len(queue) <= 0:
                    print("UNDERFLOW")
            else:
                    queue.pop(0)



        elif user_input == 3:
            print(queue)

        else:
            print("Invalid Syntax.Please Try Again!")

#contributed by Randrita Sarkar



```

    Enter the maximum length of the queue:3
    Choose the operation you want to perform :
    1.enqueue()
    2.dequeue()
    3.display()
    
    4.exit()
    Choose the operation : 1
    Enter the element you want to add in a queue: 10
    Choose the operation : 1
    Enter the element you want to add in a queue: 20
    Choose the operation : 1
    Enter the element you want to add in a queue: 30
    Choose the operation : 3
    [10, 20, 30]
    Choose the operation : 2
    Choose the operation : 2
    Choose the operation : 3
    [30]
    Choose the operation : 4
    Operation Exist
    


```python

```
