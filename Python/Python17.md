### 짝수 숫자만 출력
#### 숫자로 구성된 하나의 리스트를 입력받아, 짝수들을 추출하여 리스트로 반환하는 pickup_even 함수를 구현하라.
```python
pickup_even([3, 4, 5, 6, 7, 8])
```
```python
[4, 6, 8]
```
```python
def pickup_even(items):
    result = []
    for item in items:
        if item % 2 == 0:
            result.append(item)
    return result
```
