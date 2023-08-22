### 버스정차문제
#### 문제

첫차 : 오전 6시  막차 : 오후 23시 운행 종료

A버스 : 15분 간격 운행

B버스 : 13분 간격 운영

첫차 : 6시 20분 막차 : 오후 22시

C버스 : 8분 간격 운행

집앞 버스 정류장에서 학교까지 가는 버스 A,B,C의 운행정보가 다음과 같을 때, 2대 이상의 버스가 정차하는 시간대를 출력해보자.
```python
stepA = 15
stepB = 13
stepC = 8

for i in range(60 * 17+1):
    if 20 < i <= 60 * 16:
        if i % stepA == 0 and i % stepC == 0:
            print(f'BUS A | BUS C 동시 운행\t : \t{(60 * 6 + i) // 60}시 {(60 * 6 + i) % 60}분 ')
        if i % stepC == 0 and i % stepB == 0:
            print(f'BUS B | BUS C 동시 운행\t : \t{(60 * 6 + i) // 60}시 {(60 * 6 + i) % 60}분 ')

    if i % stepA == 0 and i % stepB == 0:
        print(f'BUS A | BUS B 동시 운행\t : \t{(60 * 6 + i) // 60}시 {(60 * 6 + i) % 60}분 ')

```
