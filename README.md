# Remove-Duplicate-Elements in python
n = int(input())
a = [int(input()) for i in range(0,n,1)]
for i in range(n):
    flag = 0
    for j in range(i, -1, -1):
        if a[i] == a[j]:
            flag += 1
    if flag == 1:
        print(a[i])
