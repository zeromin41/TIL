### 시리즈
판다스 라이브러리를 통해 리스트를 시리즈로 만들수 있음.

```python
import numpy as np
import pandas as pd

s = pd.Series([1, 3, 5, np.nan, 6, 8])
s
```
```python
0    1.0
1    3.0
2    5.0
3    NaN
4    6.0
5    8.0
dtype: float64
```
### 데이터프레임
인덱스와 열라벨을 설정하여 데이터프레임을 만들수있음.

```python
dates = pd.date_range(start="20130101", periods=6)
dates
```
```python
DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
               '2013-01-05', '2013-01-06'],
              dtype='datetime64[ns]', freq='D')
```
이 데이터프레임에서 열라벨을 따로 ABCD로 지정해주고, 인덱스도 dates로 지정해주면 원하는 모양의 데이터프레임을 생성할수있다.

```python
np.random.seed(0)

df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))
df
```
