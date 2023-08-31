#### iloc 

1. 데이터프레임의 행이나 컬럼에 인덱스 값으로 접근.

2. integer location의 약어로, 컴퓨터가 읽을 수 있는 indexing 값으로 데이터에 접근하는 것이다.

#### loc

1. 데이터프레임의 행이나 컬럼에 label이나 boolean array로 접근.

2. location의 약어로, 인간이 읽을 수 있는 label 값으로 데이터에 접근하는 것이다.

```python
import pandas as pd

df = pd.DataFrame({
    "bid_id": [1, 2, 3],
    "bidder_id": ["Gadi", "Conda", "Lion"],
    "city": ["Seoul", "LA", "Sydney"],
    "item": ["TV", "jewelry", "book"]}).set_index("bid_id")
df
```
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FdIHsHe%2FbtqX1pBwG7Q%2FyynKb2iKWqivlMerU1qve1%2Fimg.png">

#### iloc 이용해서 접근
첫번째 행에 접근한다.
```python
df.iloc[0]
```
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcgJRDW%2FbtqX6gYjjfv%2FK1LocCOH7okhEqEEd6fCUk%2Fimg.png">

#### loc 이용해서 접근
레이블이 1인행에 대해 접근한다.
```python
df.loc[1]
```
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbVwn0E%2FbtqXXiYeDME%2FVwxCAeJv07njkrWOrb44uK%2Fimg.png">
