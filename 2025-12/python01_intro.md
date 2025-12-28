[python 기초 정리](2025-12/python01_intro.md)

## 1. Python이란?

Python은 읽기 쉽고 간결한 문법을 가진 프로그래밍 언어로,
웹 개발, 데이터 분석, 자동화, 클라우드, AI 등 다양한 분야에서 사용된다.

특히 입문자가 배우기에 부담이 적고,
실무에서도 널리 사용된다는 점이 큰 장점이다.


## 2. 변수와 자료형

### 2.1 변수 (Variable)

변수는 값을 저장하는 공간이다.
Python에서는 자료형을 따로 선언하지 않아도 된다.

```python
age = 25
name = "Python"
is_student = True
```

---

### 2.2 기본 자료형

#### 숫자형 (int, float)

```python
a = 10        # int
b = 3.14      # float
```

#### 문자열 (str)

```python
message = "Hello, Python"
```

#### 불리언 (bool)

```python
is_active = False
```

---

### 2.3 컬렉션 자료형

#### 리스트 (list) – 순서 O, 변경 O

```python
numbers = [1, 2, 3, 4]
numbers.append(5)
```

#### 튜플 (tuple) – 순서 O, 변경 X

```python
point = (10, 20)
```

#### 딕셔너리 (dict) – key-value

```python
user = {
    "name": "Kim",
    "age": 25
}
```

#### 집합 (set) – 중복 X

```python
unique_numbers = {1, 2, 3, 3}
```

---

## 3. 조건문 (if)

조건에 따라 다른 동작을 수행할 수 있다.

```python
score = 85

if score >= 90:
    print("A")
elif score >= 80:
    print("B")
else:
    print("C")
```

---

## 4. 반복문 (for, while)

### 4.1 for 문

```python
for i in range(3):
    print(i)
```

### 4.2 while 문

```python
count = 0

while count < 3:
    print(count)
    count += 1
```

---

## 5. 함수 (Function)

함수는 코드를 재사용하기 위한 구조이다.

```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)
```

---

## 6. 입력과 출력

### 6.1 출력 (print)

```python
print("Hello World")
```

### 6.2 입력 (input)

```python
name = input("이름을 입력하세요: ")
print("안녕하세요,", name)
```

---

## 7. 클래스 (Class) 기초

클래스는 객체를 만들기 위한 설계도이다.

```python
class Person:
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def introduce(self):
        print(f"이름은 {self.name}, 나이는 {self.age}입니다.")

p1 = Person("Kim", 25)
p1.introduce()
```
