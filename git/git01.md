#### git ignore
git에 올릴 파일 중 삭제하지 않고 무시하는 파일

파일 생성
```
touch [파일]
```

.gitignore 파일 생성
```
touch [.gitignore]
```

무시할 파일들을 .gitignore 파일로 추가
```
echo "[무시할 파일]" >> .gitignore
```

ignored된 파일 보는법
```
git ls-files --other --ignored --exclude-standar    #shell script로 작성
```

--other : 추적되지 않는 파일 표시

--igcored : 출력에서 무시 된 파일만 표시

--exclude-standard : 표준 git 제외를 추가함

#### git add

git add는 작업 디렉토리상의 변경 내용을 스테이징 영역에 추가하기 위해 사용하는 Git 명령어. 

파일과 폴더를 모두 arguments로 받음. 

또한 git add는 Untracked상태의 파일을 Tracked상태롤 바꿀때와 not staged상태의 파일을 staged상태로 바꾸어줄때 사용함.

#### git reset

add된 파일이나 디렉토리들을 전부 지워줌.

#### git commit

staged한 파일들을 직접적으로 저장소에 올리는 역할.

#### git status

작업 디렉토리와 스테이징 영역의 상태를 확인

* Changes to be committed : 커밋이 되기위한 변경사항 (git add된 파일들)
* Changes not staged for commit : 변경한 git add 되지 않은 파일들
* Untracked files : Untracked File은 Git 저장소에는 있지만 Git에 의해서 관리되고 있지 않은 파일입니다.

#### git clone

git 원격 저장소를 로컬로 복제하는 명령어

```
git clone [원격 저장소] [원격 저장소를 복제할 파일]
```

위 명령어를 실행하면 빈 파일에 원격 저장소가 복제됨.

그리고 올리려는 파일들을 해당 파일에 넣어줌.

```
mv [올릴 파일] [원격 저장소가 복제된 파일]
```

그러면 [원격 저장소가 복제된 파일]에 ls -a 를 해주면 .git 파일이 있는 것을 확인할 수 있음.

이후 [원격 저장소가 복제된 파일]로 이동하여 git add* 를 해서 stage를 해준다.

마지막으로 git push 해주면 원격 저장소에 올라감.
