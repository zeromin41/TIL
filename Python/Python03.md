#### 리스트

list() 함수는 튜플, 문자열 모음 등을 리스트 형식으로 변환함.
```
tup = ('foo', 'bar', 'baz')
b_list = list(tup)
```
```
b_list
```
```
['foo', 'bar', 'baz']
```
* 리스트 변경
  ```
  b_list[1] = 'peekaboo'
  b_list
  ```
  ```
  ['foo', 'peekaboo', 'baz']
  ```
* 리스트 추가
  ```
  b_list.append('dwarf')
  b_list
  ```
  가장 오른쪽에 추가됨.
  ```
  ['foo', 'peekaboo', 'baz', 'dwarf']
  ```
* 리스트 추가 (자리 지정)
  ```
  b_list.insert(1, 'red')
  b_list
  ```
  1번 인덱스에 추가됨
  ```
  ['foo', 'red', 'peekaboo', 'baz', 'dwarf']
  ```
* 리스트 삭제
  ```
  b_list.pop(2)
  ```
  삭제하기전에 삭제되는 값을 반환함.
  ```
  'peekaboo'
  ```
  ```
  b_list
  ```
  ```
  ['foo', 'red', 'baz']
  ```
* 리스트 삭제 (지정 항목 삭제)
  ```
  b_list.insert(1, 'foo')

  b_list.remove('foo')
  b_list
  ```
  중복된 값이 있으면 가장 작은 인덱스에 위치한 값이 삭제됨.
  ```
  ['foo', 'red', 'baz']
  ```
* 리스트 이어붙이기
  * '+'로 이어붙이기
    새로운 이어진 리스트가 생성됨.
  * extend() 메서드 이용
 
    원래의 리스트를 이어붙인 리스트로 수정하는 메서드.
    ```
    x = [4, None, 'foo']
    x.extend([5, 8, (2, 3)])
    ```
    ```
    x
    ```
    ```
    [4, None, 'foo', 5, 8, (2, 3)]
    ```
* 리스트 정렬
  ```
  a = [9, 2, 5, 1, 3]
  a.sort()
  ```
  ```
  a
  ```
  ```
  [1, 2, 3, 5, 9]
  ```
  키워드 인자를 이용해 정렬 기준을 설정 할 수 있음.
  ```
  b = ['sox', 'small', 'be', 'a']
  b.sort(key=len)
  b
  ```
  ```
  ['a', 'be', 'sox', 'small']
  ```
* 리스트 슬라이싱 (튜플, 문자열 동일)
  ```
  seq = [7, 2, 3, 6, 5, 6, 0, 1]
  sub_seq = seq[1:5]

  sub_seq
  ```
  ```
  [2, 3, 6, 5]
  ```
  음수 슬라이싱은은 뒤에서 부터 적용
  ```
  seq[-4:]
  ```
  ```
  [6, 5, 6, 0, 1]
  ```
  
  스텝 사용 가능
  ```
  seq[::2]
  ```
  ```
  [7, 3, 5, 0]
  ```
  
