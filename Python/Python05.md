### 리스트와 튜플 차이 

리스트는 기본적으로 요소들을 변경할 수 있지만 튜플은 불가능함

```python
# 리스트 생성
my_list = [1, 2, 3, 4, 5]
print("리스트:", my_list)

# 튜플 생성
my_tuple = (6, 7, 8, 9, 10)
print("튜플:", my_tuple)

# 리스트의 항목 변경
my_list[2] = 33
print("변경된 리스트:", my_list)

# 튜플의 슬라이싱 (변경x, 선택0)
subset_of_tuple = my_tuple[1:4]
print("튜플 일부 선택:", subset_of_tuple)

# 튜플과 리스트의 길이 구하기
list_length = len(my_list)
tuple_length = len(my_tuple)
print("리스트 길이:", list_length)
print("튜플 길이:", tuple_length)

# 리스트와 튜플의 반복
for item in my_list:
    print("리스트 항목:", item)

for item in my_tuple:
    print("튜플 항목:", item)

# 리스트에 항목 추가
my_list.append(6)
print("항목 추가된 리스트:", my_list)

# 튜플과 리스트 비교
if 7 in my_tuple:
    print("튜플에 7이 있습니다.")

if 7 in my_list:
    print("리스트에 7이 있습니다.")
```

이처럼 리스트는 직접 리스트에 접근하여 변경이 가능하지만 튜플은 슬라이싱하거나 인덱싱하여 부분선택하는 것만 가능함.

```Python
리스트: [1, 2, 3, 4, 5]
튜플: (6, 7, 8, 9, 10)
변경된 리스트: [1, 2, 33, 4, 5]
튜플 일부 선택: (7, 8, 9)
리스트 길이: 5
튜플 길이: 5
리스트 항목: 1
리스트 항목: 2
리스트 항목: 33
리스트 항목: 4
리스트 항목: 5
튜플 항목: 6
튜플 항목: 7
튜플 항목: 8
튜플 항목: 9
튜플 항목: 10
항목 추가된 리스트: [1, 2, 33, 4, 5, 6]
튜플에 7이 있습니다.
리스트에 7이 있습니다.
```
