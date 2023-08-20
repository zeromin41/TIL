### 어레이 변형

reshape() 메서드를 활용하여 주어진 어레이의 모양을 원하는 대로 변형이 가능함. 단, 항목의 수가 변하지 않도록 모양을 지정해야 함.

```python
arr = np.arange(8)
arr
```
```python
array([0, 1, 2, 3, 4, 5, 6, 7])
```
```python
arr.reshape((4, 2))
```
```python
array([[0, 1],
       [2, 3],
       [4, 5],
       [6, 7]])
```
