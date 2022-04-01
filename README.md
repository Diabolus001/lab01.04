# lab01.04
Задание 1
def distance(x1, y1, x2, y2):
    return sqrt((x1 - x2) ** 2 + (y1 - y2)** 2)

x1 = float(input())
x2 = float(input())
y1 = float(input())
y2 = float(input())
print(distance(x1, x2, y1, y2))
Задание 2
a = int(input())
b = int(input())
c = int(input())
d = int(input())

def min4(a, b, c, d):
    return min(min(min(a, b), c), d)

print(min4(a, b, c, d))
Задание 3
def IsPointInSquare(x, y): #Основная программа должна считать координаты точки 
    return (abs(x) <= 1) and (abs(y) <= 1) #завершает функцию и возвращает значение


x = float(input())
y = float(input())
if (IsPointInSquare(x, y)):
    print('YES')
else:
    print('NO')
Задание 4
def IsPointInSquare(x, y):
    if x ** 2 + y ** 2 <= 2 ** (1/2):
        return True

x = float(input())
y = float(input())
if IsPointInSquare(x, y):
    print("YES")
else:
    print("NO")
Задание 6
def power(a,n):
    if n == 0:
        return 1
    else:
        return a * power(a, n - 1)
print(power(float(input()), int(input())))
Задание 7
def ReducefFranction(n, m):
    p1 = max(n, m)
    p2 = min(n, m)
    if p1 == p2 and p1 * p2:
        return 1, 1
    else:
        p = p1 % p2
        while p>0:
            p1 = p2
            p2 = p
            p = p1 % p2
        return n // p2, m // p2
n = int(input())
m = int(input())
print(ReducefFranction(n, m))
