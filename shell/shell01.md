### 파일 이동
```
mv -옵션 [이동시키려는 파일 또는 디렉토리] [이동시킬 곳]
```
현재 디렉토리안에 있는 전체 파일을 상위 폴더로 이동
```
mv * ../
```
옵션

* -b : 이동 시킬 곳에 이미 파일 혹은 디렉토리가 있다면 옮기기전에 백업하고 이동.
* -f : 이동 시킬 곳에 이미 파일 혹은 디렉토리가 있다면 묻지도 따지지도 말고 그냥 강제 이동.
* -i : 이동 시킬 곳에 이미 파일 혹은 디렉토리가 있다면 일단 묻기.
* -v : 이동시키는 과정을 보여줌.

### 파일 삭제
```
rm -옵션 [삭제할 파일 또는 디렉토리]
```
가장 자주 쓰이는 코드로 삭제 후 메세지 안뜸
```
rm -rf [삭제할 파일 또는 디렉토리]
```
옵션

* -f : 강제로 파일이나 디렉토리를 삭제하고 대상이 없는 경우에는 메시지를 출력X
* -r : 디렉토리 내부의 모든 내용을 삭제
* -d : 비어있는 디렉토리들만 제거
* -i : 매번 삭제할때마다 사용자에게 삭제할것인지 묻기.
* -l : 3개의 이상의 파일을 삭제하거나 디렉토리 내부가 비어있지 않을때만 삭제할것인지 묻기.
* -v : 삭제되는 대상의 정보를 출력.
