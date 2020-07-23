# GitHub Tutorial - Git

## 0. git 이란?

개발자의 코드를 항상 지켜보는 도구

가면 갈수록 점점 더 복잡하고 관리하기 힘든 코드를 다루는데 도움을 줄 강력한 도구

팀 프로젝트에 있어서 협업을 도와 줄 수 있는 유용한 도구

## 1. git 설치

  * wsl 설치
  
  * wsl에서 ```sudo apt-get install git``` 입력
  
  * ```git --version``` 으로 제대로 설치 되었는지 확인 
  
  * 2.25.1이 나오면 정상적인 설치 완료
  
  * ```git init``` 입력 (git 초기화)
  
  * ``` git config --global user.email “email”``` <br/>
    ```git config --global user.name “name”  ``` 입력
  
## 2. Git <-> Local

  * VsCode 설치
  
  * WorkSpace 설정 (= 작업할 폴더 생성)
  
  * VsCode에서 workspace 진입
  
  * 아무 파일이나 생성
  
  * ```git add example.html``` 입력
  
  * 파일 내용 수정 (수정할 때 branch 사용 가능) [branch 내용 보러가기](#브랜치branch) 
  
  * ```vim example.html```을 입력해 변화 확인
  
  * ```git add example.html``` 입력
  
  * ```git diff``` 입력을 통해 변화 확인
  
  * ```git commit example.html``` (최종 파일을 로컬 저장소로 보내기)
 
## 3. Local <-> github
  
  * ```git remote add origin 원격저장소 주소``` 입력
  
  * ```git clone origin``` <-- 처음 서버에서 정보를 받을 때     ```git pull origin``` <-- 그 후 {두 경우 모두 작업 하기 전 서버와 동기화 시키는 명령어}
  
  * 작업
  
  * ```git push -u origin master``` 입력 
  
    * `origin` : 등록한 원격저장소 주소  `master` : 본인의 브랜치이자 깃허브 사이트에 올라가는 브랜치 이름
    


### 브랜치(branch)
```
원할한 파일 변경을 위해 만들어진 방법

초기화 되있는 상태에선 branch가 master 하나 뿐이지만, git branch branch_name 과 같은 방법으로 branch를 늘릴 수 있다.
git checkout branch_name을 입력하면 브랜치가 master에서 issue1으로 변경된다. branch 생성과 변경 동시에 하려면 git checkout -b branch_name을 입력하면 된다. (-b 옵션)
사용하는 일례로, issue1 브랜치를 생성 후, 작업을 진행한 후 master 브랜치에 git checkout master , git merge issue1 2개의 명령어를 사용하여 병합할 수 있다.  
이렇게 하면 master에 직접 수정하는 것보다 위험 부담이 작아진다.
```
  
