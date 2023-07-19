#### cat 명령어

cat은 파일 내용을 출력하는 명령어임.
```
cat -옵션 [파일]
```
옵션

* -n        : 모든 라인 앞에 라인 번호 출력. (빈 라인도 번호 출력)
* -b        : 비어 있지 않은 라인에만 번호 출력.
* -E        : 라인의 마지막에 $ 기호 출력. (빈 라인도 $ 기호 출력)
* -T        : 탭 문자를 ^I로 바꿔서 출력.
* -s        : 두 번 이상 연속된 빈 라인(empty line) 출력 안함.
* -v        : 탭(TAB)과 줄바꿈(LFD)을 제외한 nonprinting 문자를 ^, M-를 사용하여 표시.
* -e        : -vE와 결과 같음. 줄바꿈(LFD)을 포함한 nonprinting 문자 표시.
* -t        : -vT와 결과 같음. 탭(TAB)을 포함한 nonprinting 문자 표시.
* -A        : -vET와 같음. 탭(TAB), 줄바꿈(LFD)을 포함한 nonprinting 문자 표시.

```
cat > [파일]

내용입력
```
입력한 내용을 가진 파일을 생성함.


```
cat [파일1] - [파일2]
```
FILE1 출력한 다음 표준 입력(-)으로 입력받은 내용 출력 후 [파일2] 내용 출력.

#### diff 명령어

두 파일을 비교하는 명령어임.

```
diff [옵션][비교파일1][비교파일2]
```
옵션

* -b  : 연속된 공백 무시
* -i   : 대소문자를 구분하지 않음
* -t   : 출력 라인에 TAB 문자를 넣음
* -w  : 두 행의 비교 시 공백을 무시
* --brief : 파일 비교 후 결과 표시(같은지, 다른지)
* -d  : 세세한 차이까지 검색
* -H  : 큰 파일을 빠르게 처리할 때 사용
* -q  : 두 파일의 차이점만 출력
* -s   : 두 파일이 같은 지 확인
* -r   : 두 디렉토리의 차이점 출력
* -u  : undirectional new file 옵션으로 비교하는 파일/디렉토리가 빠져있을 경우 dummy로 처리해서 출력을 통일시킴
* -r   : recursive 하위 디렉토리 모두 검색
* -N  : 검색 중 new file도 적용 가능

```
1a2
```

1 : 원본 파일의 line 수 (~1번째 line)

a : added (추가)

2 : 수정한 결과 line 수 (1 line 에서 한 줄 추가해서 2 line 이 됨)

```
3d2
```

3 : 원본 파일의 line 수 (~3번째 line)

d : deleted (삭제)

2 : 수정한 결과 line 수 (3 line 에서 한줄 삭제해서 2 line 이 됨)

#### find 명령어

```
find [경로] [옵션]
```

계층구조로 이루어진 디렉토리 내에 존재하는 파일들을 검색 하는 기능

* -type
   특정 디렉토리 내의 특정 타입에 해당하는 파일들을 찾음
  * -l : 심볼릭 링크 파일
  * -f : 일반 파일
  * -d : 디렉토리
* -name
   파일명으로 검색
  * . : 현재 Path를 시작지점으로 지정
  * [] : 파일명으로 올 수 있는 문자의 종류 및 순서, 범위를 지정 (정규식과 유사)
  * ? : 한 글자를 의미, 어떠한 문자도 올 수 있음
 
  ex
  ```
  # image.img 파일을 찾을 때
  $ find . -name image.img

  # m1.jpg, m2.jpg 와 같이 "m + 한글자 숫자" 를 찾을 때
  $ find . -name 'm?.jpg'

  # json 파일 전부 찾고 싶을 떄
  $ find . -name *.json

  # 디렉토리중 te 로 시작하는 목록
  $ find . -type d -name '[t][e]*'
  ```
* -size
  파일 사이즈로 검색
  * c : byte
  * w : 2 byte word
  * k : Kilobytes
  * M : Megabytes
  * G : Gigabytes
 
* atime : access time
* ctime : creation time
* mtime : modification time

  * -n : n day or (24 x n)
