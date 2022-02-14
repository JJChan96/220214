# Git 기초

Project 폴더 -> C:\Users\pc-007\Document\workspace\leacure
Project 폴더에서 src를 가라! -> C:\Users\pc-007\Document\workspace\leacure\src

src에 있는 상태에서 root 디렉토리로 가라! ->
C:\Users\pc-007\Document\workspace\leacure

Project 폴더에서 git init을 써라 
-> 앞으로 leacure 디렉토리는 git로 관리하겠다.


git 도움을 주는 확장앱 설치
1. Git Graph 설치


먼저 Git Graph를 보기전에 git init을 통해 .git을 만들고 commit을 해보자 

내가 commit한 내용을 보고 싶으면 'git log'를 치면 확인할 수 있다.

git log를 치면 commit 한 내용들이 나타날텐데 옆에 (HEAD -> master)라고 뜰 것이다. 이 의미는 내가 지금 해당 내용을 중점적으로 보고있다?라고 생각하면 된다.


commit 옆에 있는 숫자와 영어 조합은 commit 의 해시값(이름)이라고 생각하면 된다.

인제 해당상태에서 벗어날려면 : q! wq!




Git Graph를 실행하는 방법 :

소스 제어(<ctrl + shipt> + g)키를 누르고 상단에 View Git Graph를 누르면 확인할 수 있다.


Git 의 장점

: 용량을 최소화하되 기능은 더 올라간다

Git 의 단점 

: 어렵다




1. gitignore

2. Reset, Revert 커밋을 뒤로 돌아가는 행위

3. branch 커밋을 나누는 행위

4. merge, rebase 커밋을 합쳐주는 행위




1. gitignore

내가 굳이 이 폴더는 Git에 올릴 필요가 없는 파일이나 디렉토리들이 있을 것이다.  ex) (node_modules, package-lock.json 등등)

이런 파일들을 제외하고 깃에 올릴 수 있는 방법을 확인해보자


1-1. 프로젝트 폴더에서 .gitignore 파일을 생성해준다.
1-2. .gitignore 파일에 node_modules를 치면 node_moules를 git을 올리는데 추적하지 않고 올리지 않게 해준다.
1-3. git status를 누르면 작성한 두 파일을 추적하지 않는 것을 확인할 수 있다.

1-4(논외, node관련). 만약에 node-modules를 지우고자 한다. 이것을 지우고 node를 실행하면 실행이 되지 않는 것을 알 수 있다. 그렇다면 node-modules를 다시 설치하고자 한다면 expres를
                    설치한것처럼 하나하나 다 설치를 해야하나?? 그렇지 않다 package.json에 dependencies안에 들어있는 것이 다 확인할 수 있다면 그저 'npm install'만 치면 dependencies에 해당되는 라이브러리를 자동으로 다 설치할 수 있다. 
                    그렇기에 우리는 깃허브에 올릴 때 gitignore을 통해서 node_modules, package-lock.json을 포함하지 않고 올린다. ( 따로 설치할 수 있으니! )

1-5 git rm -r [파일명]  : 로컬과 원격저장소를 다 지움
    git rm --cached -r [파일명] : 원격저장소에서만 지움


아래 3개를 하기전 text 저장소를 하나 만들어보자

2. Reset, Revert 커밋을 뒤로 돌아가는 행위

3. branch 커밋을 나누는 행위

4. merge, rebase 커밋을 합쳐주는 행위


