#### git clone
```
git clone [REPO_URL] [DIR]
```
클론한 온라인 저장소 주소를 지정함. 

[DIR] 는 저장소를 로컬에 복제할 위치를 지정함. (생략가능)

#### ssh

로컬 개발 환경에서 Git을 단독으로 사용한다면 SSH가 없어도 무방하지만, 안전하게 외부 Git 서버에서 코드를 Clone하거나 Push하려면 SSH 프로토콜을 사용해야함. 
GitHub처럼 인터넷을 통해 원격에서 Git 저장소를 호스팅해주는 서비스에서도 SSH 프로토콜을 지원함. GitHub 뿐만 아니라 원격 Git 저장소와 통신할 때 일반적으로 사용하는 방법임.

ssh 키를 생성한 적이 있는지 확인하는 코드
```
$ cd ~/.ssh
$ ls
```
id_ed25519와 id_ed25519.pub 혹은 id_rsa와 id_rsa.pub 파일쌍이 있으면 키가 있는 것임.

키 생성 코드
```
$ ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
```

#### git 명령어

* git init
* git status : 상태 확인
* git add
--update : 추적하고 있는 파일만 add
* git rm : 제거 관련 명령어
--cached : add된 파일 제거 ( 해당 파일을 working directory 상태로 되돌림 )
* git commit
-m : 간단한 커밋 메시지 작성
--amend : 마지막 커밋 메시지 수정
* git checkout
-- {file} : working directory에서 작업한 내용을 버림
* git push : 로컬 브랜치(local branch)를 원격 저장소(remote repository)로 푸시
* git ls-files : git 에 의해 추적되는 모든 파일을 표시
