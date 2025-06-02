---
layout: post
title: 100 bài code pytho thiếu nhi(P2)
subtitle: 
tags: [python]
author: vuthilinh
---

Hôm nay chúng ta tiếp tục seri luyện code python với 100 bài code thiếu nhi nhé! vì mình học bên Trung nên từ bài này trở đi, ngoài phần ghi chú tiếng anh, mình sẽ thêm vào một sô từ tiếng Trung nữa nhé, để mình ghi nhớ khi phải nói với các thầy cô bên Trung thui kakaka, nếu k thích bạn cứ bỏ qua các chữ đó nhé !!
	Let's go!~
# 2. BÀI TẬP LỆNH ĐIỀU KIỆN CƠ BẢN
## 2.1. Bài 13
Nhập vào số nguyên dương a, nếu a lớn hơn 10 thì ta in ra đây là số lớn hơn 10.
```python
while True:
	a = int(input("Input a = "))
	if a>0:
		break  # thoát vòng lặp while
	else:
		print("a must be a positive interger（正整数） number! )
if a>10:
	print("a is greater than(大于) 10")
```
Kết quả:
```bash
Input a = -2 
a must be a positive interger number! 
Input a = 7
```
## 2. 2. Bài 14
Nhập vào số nguyên dương a, nếu a là số chẵn thì in ra đây là số chẵn, ngược lại in ra đây là số lẻ.
```python
While True:
	a = int(input("Input（输入） a = "))
	if a>0:
		break # thoát vòng lặp while
	else:
		print("a must be a positive integer number!)
	if a%2==0:
		print("a is a even number(偶数)")
	else: 
		print("a is a odd number(奇数)")
```
Kết quả (结果)：
```bash
Input（输入） a = -3 
a must be a positive integer number! 
Input（输入） a = 10 
a is a even number(偶数)
```
## 2.3. Bài 15
Nhập vào 3 số thực dương a, b, c. Kiểm tra xem a, b, c có cấu thành độ dài của 1 tam giác được không.
	Để a,b,c cấu thành 1 tam giác thì phải đảm bảo tổng 2 cạnh lớn hơn cạnh còn lại.
```python
while True:
	a = float(input("Input positive float number a = "))
	b = float(input("Input positive float number b = "))
	c = float(input("Input positive float number c = "))
	if a>0 and b>0 and c>0:
		break
	else:
		print("a,b,c is positive float number")
if (a+b)>c or (a+c)>b or (b+c)>a:
	print("a,b,c could create a strangle")
else:
	print("a,b,c clouldn't create a strangle")
```
Kết quả:
```bash
Input positive float number a = -2 
Input positive float number b = 4 
Input positive float number c = 6 
a,b,c is positive float number 
Input positive float number a = 2 
Input positive float number b = 5 
Input positive float number c = 3 
a,b,c could create a strangle
```
## 2.4. Bài 16
Từ bài số 15, nếu a, b, c cấu tạo thành được một tam giác, kiểm tra xem đó là tam giác gì (tam giác đều, tam giác vuông cân, tam giác vuông, tam giác cân hay tam giác thường).
```python
while True:
	a = float(input("Input positive float number a = "))
	b = float(input("Input positive float number b = "))
	c = float(input("Input positive float number c = "))
	if a>0 and b>0 and c>0:
		break
	else:
		print("a,b,c is positive float number")
if (a+b)>c or (a+c)>b or (b+c)>a:
	print("a,b,c could create a triangle")
	if a==b==c:
		print(" and abc is isosceles triangle(等腰三角形)")
	elif abs(a**2 + b**2 - c**2) < 1e-6:
		print("abc is right triangle(直角三角形)")
	else:
		print("abc is scalene triangle(不等边三角形)")
else:
	print("a,b,c clouldn't create a triangle")
```
Kết quả:
```bash
Input positive float number a = 6
Input positive float number b = 6
Input positive float number c = 6
a,b,c could create a triangle
 and abc is isosceles triangle(等腰三角形)
```
## 2.5. Bài 17
Nhập vào 3 số a, b, c. Hãy sắp xếp 3 số a, b, c theo thứ tự tăng dần rồi in ra lại.
```python
a = float(input("Input a = "))
b = float(input("Input b = "))
c = float(input("Input c = "))
d= 0
if a>b:
	d = b
	b = a
	a = d
if a>c:
	d = c
	a = c
	c = d
if b>c:
	d = c
	c = b
	b = d	
print("3 số theo thứ tự tăng dần là:", a, b, c)
```
Kết quả
```bash
Input a = 4 
Input b = 1 
Input c = 8 
3 số theo thứ tự tăng dần là: 1.0 4.0 8.0
```
## 2.6. Bài 18
Giải và biện luận phương trình ax + b = 0
```python
a = float(input("Nhập a = "))
b = float(input("Nhập b = "))
if a==0:
	if b==0:
		print("ptr vô số nghiệm")
	else:
		print("ptr vô nghiệm")
else:
	x = -b/a
	print("Kết quả của phương trình %.2f x+%.2f=0 là: x = %2.f" %(a,b,x))
```
Kết quả:
```bash
Nhập a = 3 
Nhập b = 6 
Kết quả của phương trình 3.00 x+6.00=0 là: x = -2
```
## 2.7. Bài 19
Giải và biện luận phương trình ax^2 + bx + c = 0
```python
import math

a = float(input("Nhập a = "))
b = float(input("Nhập b = "))
c = float(input("Nhập c = "))

if a == 0:
    if b == 0:
        if c == 0:
            print("Phương trình có vô số nghiệm (0 = 0).")
        else:
            print("Phương trình vô nghiệm (hằng số khác 0).")
    else:
        x = -c / b
        print(f"Phương trình bậc nhất, có nghiệm: x = {x:.2f}")
else:
    delta = b**2 - 4*a*c
    print(f"Δ = {delta:.2f}")
    if delta < 0:
        print("Phương trình vô nghiệm (không có nghiệm thực).")
    elif delta == 0:
        x = -b / (2*a)
        print(f"Phương trình có nghiệm kép: x = {x:.2f}")
    else:
        sqrt_delta = math.sqrt(delta)
        x1 = (-b + sqrt_delta) / (2*a)
        x2 = (-b - sqrt_delta) / (2*a)
        print("Phương trình có 2 nghiệm phân biệt:")
        print(f"x₁ = {x1:.2f}")
        print(f"x₂ = {x2:.2f}")
```
Kết quả:
```bash
Nhập a = 6 
Nhập b = 7 
Nhập c = 9 
Δ = -167.00 
Phương trình vô nghiệm (không có nghiệm thực).
```
Tạm thời hôm nay đến đây nhé, hẹn các bạn ở phần tiếp theo!
	

