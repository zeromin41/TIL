### 문자열 다루는 기본 함수

#### 문자열 대/소문자 변환 : upper, lower, title, capitalize

upper은 모든 문자를 대문자로,

lower은 모든 문자를 소문자로,

title은 각 단어의 첫 글자를 대문자로, 나머지는 소문자로,

그리고 capitalize는 첫 글자만 대문자로, 나머지는 소문자로 바꿈.

영단어 외의 다른 문자는 바뀌지 않고 반환됨.

#### 문자열 탐색 : count, find, index

문자열에서 특정 정보를 탐색할 수 있는 함수임.

count 함수는 특정 문자의 개수를 반환.

find 함수는 해당 문자가 처음으로 등장하는 인덱스를 반환.

index 함수는 find 함수와는 사용법이 거의 동일하나, 해당 문자를 찾지 못하면 -1을 반환하는 것이 아니라, 에러를 발생.

#### 문자열 구성 파악 : isdigit, isalpha, isupper, islower

isdigit은 모든 문자열이 숫자이면 True,

isalpha는 모두 알파벳이거나 한글이면 True,

isupper, islower은 각각 모두 대문자, 소문자로 구성인지 여부로 True를 반환.

#### 문자열 공백 제거, 특정 문자 대체 : strip, rstrip, lstrip, replace

문자열에서 공백을 제거할 수 있는 함수들은 strip, rstrip, lstrip이 있고 줄바꿈 문자(\n)이나 tab문자(\t) 등도 포함하여 제거가 가능.

rstrip은 오른쪽 끝, lstrip은 왼쪽 끝의 공백을 제거하며, strip 함수는 양쪽 끝의 공백을 모두 제거함.

replace 함수는 특정 문자를 다른 문자로 대체함.

#### 문자열 쪼개기, 합치기 : split, join

split은 문자열을 공백 등으로 나눠서 단어 단위로 쪼개어 리스트에 반환.

join은 리스트에 들어있는 단어들을 하나의 문자열로 원하는 모양으로 합침.
