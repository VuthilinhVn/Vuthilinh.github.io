---
layout: post
title: 100 bài code python thiếu nhi(P1)
subtitle: Cùng nhau học code
tags: [python]
author: vuthilinh
---

Để luyện code thì k còn cách nào khác đó là "Làm nhiều quen tay" cả, vì thế ở seri này chúng ta cùng nhau luyện 100 bài code python thiếu nhi nhé các bạn. 
	
# P1. Bài tập nhập liệu và toán tử cơ bản
## 1.1. Bài 1:
Nhập vào số n, hãy nhân n lên cho 3, rồi cộng 1 sau đó in kết quả ra màn hình.

```python
n = input("Input n = ") # vì nhập vào từ bàn phím mặc định là kiểu str

n = float(n)  #ép kiểu

result = n*3 + 1

print(f"Result is: {result}")
```
Kết quả
```bash
Input n = 3

Result is: 10.0
```
## 1.2. Bài 2
Nhập vào số n, hãy mũ 2 rồi chia cho 3, sau đó in kết quả ra màn hình

```python
n = input("Input n = ") # vì nhập vào từ bàn phím mặc định là kiểu str

n = float(n)  #ép kiểu

result = (n**2)/3

print(f"Result is: {result}")
```
Kết quả
```bash
Input n = 3 
Result is: 3.0
```
## 1.3. Bài 3
Nhập vào nhiệt độ c, in ra nhiệt độ F

```python
c = input("Nhiet do c = ")
c = float(c)
result = c*1.8 + 32 # công thức chuyển độ C sang độ F
print(result)
```
Kết quả:
```bash
Nhiet do c = 35 
Nhiệt độ F là: 95.0
```
## 1.4. Bài 4
Nhập vào một số nguyên a, nếu a chia hết cho 2 thì in ra True, ngược lại in ra False

```python
a = input("Input a= ")
a = int(a)
a%2==0 # phép chia lấy phần dư
```
Kết quả:
```bash
Input a= 3
False
Input a= 2
True
```
# 1.5. Bài 5
Nhập vào số nguyên a, nếu a là số chia hết cho 3 và nằm trong khoảng từ 50 - 100 thì in ra True, ngược lại in ra False
```python
a = int(input("Input a = "))
if a%3==0 and (50<=a<=100):
	print("True")
else:
	print("False")

```
Kết quả:
```bash
Input a = 90 
True
Input a = 120 
False
```
# 1.6. Bài 6
Nhập vào số nguyên a, nếu a là số chia hết cho 5 nhưng KHÔNG nằm trong khoảng từ 20 - 70 thì in ra True, ngược lại in ra False
```python
a = int(input("Input a = "))
if a%5==0 and not (20<=a<=70):
  print("True")
else:
  print("False")

```
Kết quả: 
```bash
Input a = 25
False
Input a = 15 
True
```
# 1.7. Bài 7
Nhập vào nguyên a và b, nếu 1 trong 2 số a và b chia hết cho 2 thì in ra True, ngược lại in ra False
```python
a = int(input("Input a = "))
b = int(input("Input b = "))
if a%2==0 or b%2==0:
	print("True")
else:
	print("False")
```
Kết quả:
```bash
Input a = 4 
Input b = 5 
True

Input a = 5 
Input b = 7 
False
```
# 1.8. Bài 8
Nhập vào số thực a, kiểm tra xem a có phải là số nguyên hay không, nếu có thì in ra True, ngược lại in ra False
```python
a = float(input("Input a = "))
print(isinstance(a, int)) # hàm isinstance(object, kiểu dữ liệu)
```
	Ở đây các bạn cũng có thể sử dụng lệnh round(a) để làm tròn nhé, rồi so sánh nó với a xem có bằng nhau không, nếu bằng -> số nguyên; nếu != thì nó là số thực đó. 
Kết quả: 
```bash
Input a = 4
True

Input a = 3.2 
False
```
# 1. 9. Bài 9
Nhập vào số nguyên a, kiểm tra xem a có phải là số chính phương hay không, nếu có thì in ra True, ngược lại in ra False
Ở đây chúng ta nhớ lại một chút kiến thức nhé, số chính phương là số nguyên mà căn bậc 2 của nó cũng là số nguyên nha. 
```python
a = int(input("Input a = "))
can = a**0.5
if can*can==a:
	print("True")
else:
	print("False")

```
Kết quả:
```bash
Input a = 4
True
Input a = 5 
False
```
# 1. 10. Bài 10
Nhập vào lương tháng này nhận được, ta phải đưa cho vợ 90% số tiền lương đó. Hãy in ra lương ta giữ lại
```python
salary = float(input("Luong thang nay = "))
print("Lương còn lại = " , salary*0.1)
```
Kết quả:
```bash
Luong thang nay = 15000000
Lương còn lại = 1500000.0
```
# 1.11.Bài 11
Nhập vào 3 số a, b, c. In ra kết quả là tổng của ba số đó
```python
a = float(input("a = "))
b = float(input("b = "))
c = float(input("c = "))
print("sum(a,b,c) = ", a+b+c)
```
Kết quả:
```bash
a = 4 
b = 6 
c = 9 
sum(a,b,c) = 19.0
```
# 1.12. Bài 12
Nhập vào 3 số a, b, c. Tính và in ra d = (a + b)^c. Nếu d là số trong khoảng từ 100 - 200 thì in ra True, ngược lại in ra False
```python
a = float(input("a = "))
b = float(input("b = "))
c = float(input("c = "))
d = (a+b)**c
if (100<=a<=200):
	print("True")
else:
	print("False")
```
Kết quả:
```bash
a = 3 
b = 2 
c = 1 
False

a = 100 
b = 1 
c = 1 
True
```
Vậy là chúng ta đã cùng nhau đi hết phần 1 của "Luyện 100 bài code pytho thiếu nhi" rồi. Hẹn gặp các bạn ở phần 2: **BÀI TẬP LỆNH ĐIỀU KIỆN CƠ BẢN** nhé
