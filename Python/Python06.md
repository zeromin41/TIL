### 함수 선언
```python
def 함수이름(위치매개변수, ..., 키워드매개변수, ...):
    함수본문
```
함수를 선언할 땐 위 코드처럼 위치매개변수와 키워드매개변수를 받고 def를 통해 함수를 선언한다.

#### 위치 매개변수
위치 매개변수란 함수에 인자를 전달받는 값.

ex. 2개의 지역변수 사용한 함수

```python
def func1(b):  #def로 함수 func1 선언
    a = []
    for i in range(5):
        a.append(i)  #a에 i추가
    
    b.extend(a)  #b에 a를확장
    return b
```
```python
print(func1([-4, -3, -2, -1]))
```
```python
[-4, -3, -2, -1, 0, 1, 2, 3, 4]
```

#### 키워드 매개변수
키워드 매개변수는 직접 매개 변수명을 지정하여 매개변수를 전달하는 방법
```python
def value_times(*values, times=1): #times=1로 기본 매개변수로 지정
	for value in values: 
		print(times * value) 

value_times(1, 2, 3, 4, times=5)  #키워드 매개변수는 위치매개변수 뒤에 씀. 
```
```python
5, 10, 15, 20
```
### 함수 반환
함수는 return을 만나면 하나의 값을 반환하는데 튜플을 이용하여 여러값을 반환할 수 도 있음.
```python
def f():
    a = 1
    b = 2
    c = 3
    return a, b, c
```
```python
(1, 2, 3)
```
