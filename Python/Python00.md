#### 변수

변수가 가리키는 값이 리스트와 같이 좀 복잡한 객체일 때는 파이썬 실행기 내부에서 변수가 해당 값을 참조함.

```
a = [1, 2, 3]
```
a는 리스트를 참조하는 것임.
```
b = a
```
b도 a와 같은 리스트를 참조함.

```
a = a + 1

print(f"a = {a}", f"b = {b}", sep="\n")
```
a값이 변하더라도 b는 a의 리스트를 참조하기에 변하지 않음
>a = 5
>
>b = 4

#### 지역변수

함수의 매개 변수 또는 함수 본문 내에서 선언된 변수
```
def append_element(some_list, element):
    data_original = some_list
    data_original.append(element)
    return data_original
```
some_list, element는 함수의 매개 변수로 선언된 지역 변수이고, data_original은 함수 본문에서 선언된 지역변수임.

#### 전역변수

함수와 상관이 없이 선언된 변수
```
data = [1, 2, 3]

append_element(data, 4)
```
>[1,2,3,4]

함수의 실행이 끝나도 data는 변형된 리스트를 가리키는 변수로 남아 있다.
