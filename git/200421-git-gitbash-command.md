### 계정 설정하는 법

git config --global user.email "메일 주소"
git config --global user.name "이름"

### 기본 구조

Wriking directory -> (add) -> Index(starging area) -> (commit) -> Local repository

git add : git 이 추적하고 있는 수정된 파일이 working directory에서 staging area에 저장된다.

git commit : staging area 에 저장됐던 파일이 local repository로 확정됩니다. commit은 "작업을 마무리 했다" 라는 버전 등록을 의미한다

### 명령어

- git init : 깃 저장소를 초기화 한다. 이것을 입력한 후에 추가적인 깃 명령어를 사용할 수 있다.

- git config : 최초에 깃을 설정할때 사용한다.

- git help : 가장 많이 사용하는 깃 명령어를 보여준다.

- git status : 저장소에 상태를 체크할 수 있다. 저장소 안에 어떤 파일이 있는지, 커밋이 필요한 변경사항이 있는지, 어떤 브랜치에서 작업하고 있는지 등..

- git branch : 새로운 브랜치를 만들고, 본인의 변경사항과 파일 추가 등의 타임라인을 만든다. 동료들과 함께 작업하고 본인의 변경사항을 원할때 사용한다.

- git add : 깃이 새 파일들을 지켜보게 한다(새 파일을 추가하진 않는다). 파일을 추가하면 깃의 저장소 "스냅샷" 에 포함된다.
	- git add * : 변경된 모들 파일 스테이징

- git commit 
	- git commit -m " " : 간단한 커밋 메세지를 작성
	- git commit --amend : 마지막 커밋 메세지를 수정

- git rm : 제거 관련 명령어
	-- cached : add 된 파일 제거 (해당 파일을 working directory 상태로 되돌림)

- git push : 나의 커밋을 github online으로 보기 원할때 이 명령어로 github에 변경사항을 "push" 한다.
	- git push -u {원격 저장소 별명} {로컬 브랜치명} : 브랜치를 추적하게 해서 이후에 git push 명령어만 입력해도 원격 저장소로 push 할수 있게 해준다.
	- git push --delete { 원격 브랜치명} : remote repository 에 있는 브랜치를 삭제한다.

- git pull : 로컬 컴퓨터에서 작업할때, 작업하고 있는 저장소의 최신 버전을 원하면, 이 명령어로 부터 변경사항을 다운로드 한다.

- mkdir : 디렉토리 만들기

- cd .. : 상위 폴더로 이동

- git log : commit 로그 확인

- rm "파일명" : 파일 삭제

- rm -r "디렉토리명" : 디렉토리 삭제

- pwd : 현재 폴더

- cd ../"폴더명" : 해당 폴더로 바로 이동

- ls -al : 숨김 폴더, 숨김 파일 보기

- git clone https://github.com/아이디/이름.git : 원격 저장소를 내 컴퓨터에 받아오기 ( 새로운 폴더를 만들어서)

- git clone https://github.com/아이디/이름.git. : 원격 저장소를 내 컴퓨터에 받아오기(현재 폴더에)

- mv {원래파일명} {바뀔 파일명} : 파일명을 바꾼다.(확장자도 바꿀 수 있다)
