---
layout: post
title: Python Cơ Bản
subtitle: Tích lỹ mỗi ngày 
tags: [python]
author: vuthilinh
---
Các bài viết trong seri học Python này đều đến từ website: [https://www.learnpython.org/](learnpython.org)
# 1. Hello, World
Python là một ngôn ngữ rất đơn giản và có cú pháp rất dễ hiểu. Trong phần này chúng ta sẽ sử dụng câu lệnh Print để in/hiển thị dòng "Hello, world" ra màn hình nhé!
```python
print("Hello, world")
```
```bash
Hello, world
```
# 2. Variables and Types Biến và kiểu dữ liệu
Bạn không cần phải khai báo biến trước khi sử dụng chúng hoặc khai báo kiểu của chúng.
	ở phần này, chúng ta sẽ tìm hiểu một số kiểu đơn giản của biến trong python:
## 2.1. Number
Python cho phép 2 loại dữ liệu cơ bản của biến số là số nguyên(intergers)-int và số thực(float)-float.
```python
my_age = 27
print("Type of my_age is: ", type(my_age))
pi = 3.14
print("Type of pi is: ", type(pi))
```
```bash
Type of my_age is: <class 'int'> 
Type of pi is: <class 'float'>
```
## 2.2.  Strings
Strings là dạng dữ liệu nằm giữa dấu nháy đơn(single quote) ' ' hoặc nháy kép(double quote) " ". Phân biệt giữa 2 kiểu nháy này chủ yếu dành cho các trường hợp kiểu như "I don't know", vậy thôi đó các bạn!
```python
name = "Vu Thi Linh"
print(name)
```
```bash
Vu Thi Linh
```
## 2.3. Lists
List là dạng danh sách giống mảng (array). Nó có thể chứa bất kỳ kiểu dữ liệu nào tùy ý.
```python
list = [1, 2, "linh", "hải" , 5, 6]
list.append(10) # thêm vào cuối list
print(list)
```
```bash
[1, 2, 'linh', 'hải', 5, 6, 10]
```
Để truy cập vào 1 phần tử của list ta sử dụng list[index] với index là stt của phần tử đó.
```python
print(list[1])
```
```bash
2
```
# 3. Basic Operators Toán tử cơ bản
Arithmetic Operators Toán tử số học
	Các toán tử số học trong python khá dễ hiểu: + cộng, - trừ, * nhân, / chia, % chia lấy phần dư, ** mũ, ...
# 4. String Formatting	 Định dạng chuỗi
	Dưới đây là chỉ định cơ bản bạn nên biết:
	- `%s - Chuỗi (hoặc bất kỳ đối tượng nào có biểu diễn chuỗi, như số)
	- `%d - Số nguyên
	- `%f - Số thực
	- `%.<number of digits>f - số chữ số đằng sau dấu . của số thực
	- `%x/%X - Số nguyên trong biểu diễn hex (chữ thường/chữ hoa)
```python
data = ("John", "Doe", 53.44)
format_string = "Hello"
print("%s %s %s your balance: %f" %(format_string, data[0], data[1], data[2]))
```
Ok, hôm nay tới đây thôi nhé, hẹn gặp các bạn vào bài tiếp theo trong seri pytho với mình nhé! 
