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

--exclude-standard : 표준 git 제외를 추가한다
