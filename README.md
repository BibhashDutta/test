# HackerEarth Practice
All the Programming questions solved

**Max Borders:**
https://www.hackerearth.com/practice/basic-programming/input-output/basics-of-input-output/practice-problems/algorithm/maximum-border-9767e14c/

t = int(input())
for i in range(t):
    n_m = input().split(" ")
    n = int(n_m[0])
    m = int(n_m[1])
    t = []
    for j in range(n):
        t.append(input())
    maxi = 0
    for k in range(n):
        curr,count = None, 0
        for char in t[k]:
            if char == "#":
                count+=1
        if count>maxi:
            maxi = count
    print(maxi)
