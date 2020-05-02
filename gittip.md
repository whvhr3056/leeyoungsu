 # git 기본 명령
    git init
        새로운 local repository 생성
    git add
        변경된 파일을 storage에 추가
    git commit
        add한 파일을 local repository에 저장 
    git push
        local repository를 remote repository에 업로드
        


commit 메시지를 작성합니다.

# 커밋 git commit -m "메시지내용"

-m 옵션은 간단하게 한줄로 메시지를 작성하기 위함이며, 긴 메시지 작성이 필요하다면 git commit 명령어만 실행하면 됩니다.


 remote 등록

remote repository를 등록합니다.

# 원격 저장소 등록 git remote add origin {remote repository 주소}

origin은 remote repository의 별칭을 의미하며, 매 번 remote repository의 주소를 입력하는 것이 귀찮으므로 별칭을 사용합니다.

일반적으로 origin을 사용합니다.

) push

commit 한 내용을 remote repository에 push( 업로드 ) 합니다.

# git push origin 브랜치 명

master는 브랜치( branch )의 이름이며, remote repository를 생성하면 기본적으로 master 브랜치가 생성됩니다.

( 참고로 브랜치는 독립적인 작업 공간을 의미하며, 브랜치 덕분에 협업이 수월해지기 때문에 꼭 알아둬야 하는 개념입니다. )


master가 아닌 다른 branch로 push 하고 싶으면, 아래와 같이 master를 특정 브랜치명으로 바꿔서 명령어를 실행하면 됩니다.

# 브랜치를 추적하고 싶다면 git checkout -b 생성할브랜치이름 원격브랜치이름처럼 해주어야 합니다.
## 깃 리모트 변경 하기

### 기존 리포지토리 깔끔하게 pull / push
```
git pull
git add .
git commit -m "clean push"
git push
```

### 기존 리포지토리 remote 제거
```
git remote remove origin
```

### 새 리포지토리 remote 추가
```
