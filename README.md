Hàm `range()` trong Python rất linh hoạt và có thể nhận **1, 2 hoặc 3 tham số**. Cụ thể:

---

### 1. `range(stop)`

* **Ý nghĩa:** Tạo dãy số bắt đầu từ 0 đến `stop - 1`.
* **Ví dụ:**

```python
for i in range(5):
    print(i)
```

**Kết quả:**

```
0
1
2
3
4
```

---

### 2. `range(start, stop)`

* **Ý nghĩa:** Tạo dãy số bắt đầu từ `start` đến `stop - 1`.
* **Ví dụ:**

```python
for i in range(2, 6):
    print(i)
```

**Kết quả:**

```
2
3
4
5
```

---

### 3. `range(start, stop, step)`

* **Ý nghĩa:** Tạo dãy số từ `start` đến gần `stop`, bước nhảy `step` (có thể là số dương hoặc âm).
* **Ví dụ:**

```python
for i in range(1, 10, 2):
    print(i)
```

**Kết quả:**

```
1
3
5
7
9
```

---

### Lưu ý:

* `start` mặc định là 0 nếu không truyền.
* `step` mặc định là 1 nếu không truyền.
* Nếu `step` là số âm, dãy số sẽ đếm ngược.
* `stop` là giá trị **không bao gồm** (exclusive).

---

### Ví dụ `step` âm:

```python
for i in range(5, 0, -1):
    print(i)
```

Kết quả:

```
5
4
3
2
1
```
---
Dưới đây là đoạn code Python đơn giản để in ra **kim tự tháp bằng dấu `*`** theo số tầng. Mỗi tầng sẽ có số dấu `*` tăng dần theo kiểu hình tam giác cân:

```python
def print_pyramid(levels):
    for i in range(1, levels + 1):
        # In khoảng trắng bên trái để căn giữa
        print(" " * (levels - i) + "* " * i)

# Ví dụ in kim tự tháp 5 tầng
print_pyramid(5)
```

**Kết quả in ra sẽ như sau:**

```
    * 
   * * 
  * * * 
 * * * * 
* * * * * 
```

---
