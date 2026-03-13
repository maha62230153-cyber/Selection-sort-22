
# Selection Sort Program

n = int(raw_input("Enter number of elements: "))
a = []

for i in range(n):
    x = int(raw_input("Enter element: "))
    a.append(x)

for i in range(n):
    min = i
    for j in range(i+1, n):
        if a[j] < a[min]:
            min = j

    temp = a[i]
    a[i] = a[min]
    a[min] = temp

print "Sorted elements are:"
for i in range(n):
    print a[i]

OUTPUT 

Enter number of elements: 5
Enter element: 25
Enter element: 10
Enter element: 40
Enter element: 5
Enter element: 30

Sorted elements are:
5
10
25
30
40
