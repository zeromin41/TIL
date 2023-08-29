### 브로드 캐스팅
모양이 서로 다른 두 어레이가 주어졌을 때 두 모양을 통일시킬 수 있다면 두 어레이의 연산이 가능하도록 도와주는 기능이다.
```python
arr = np.arange(6).reshape((2,3))
arr
```
```python
array([[0, 1, 2],
       [3, 4, 5]])
```
```python
arr * 4
```
```python
array([[ 0,  4,  8],
       [12, 16, 20]])
```
정수 4로 채워진 동일한 모양의 어레이를 먼저 생성한 후에 항목별 곱셈을 진행한다.

브로드캐스팅을 통한 연산도 가능함.

ex. 어레이 더하는 연산.

```python
arr2 = np.arange(4).reshape((4,1)).repeat(3,axis=1)
arr2
```
```python
array([[0, 0, 0],
       [1, 1, 1],
       [2, 2, 2],
       [3, 3, 3]])
```
```python
arr3 = np.arange(1, 4)
arr3
```
```python
array([1, 2, 3])
```
```python
arr2 + arr3
```
```python
array([[1, 2, 3],
       [2, 3, 4],
       [3, 4, 5],
       [4, 5, 6]])
```
