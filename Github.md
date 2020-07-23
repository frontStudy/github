
# GitHub Tutorial - GitHub

## 0. github란?

git의 원격 저장소

여러 사람이 서로의 코드를 보고 고쳐주는 서버

팀 프로젝트 (혹은 오픈 소스 프로젝트)의 성지

## 1. repository란?

  * 직역하면 저장소
  
  * create repository를 클릭 후 저장소 생성
  
  * clone 후 작업 시작
  
## 2. team project

  * __issue__ : 프로젝트를 진행하다가 잡다한 특이점(요구사항, 에러, 등등)을 올리는 곳 
  
  * __pull request__ : 팀 구성원이 원격 저장소로 commit 했더라도, <br/>
                       본인이 pull-request를 신청하여 다른 팀 구성원으로 하여금 검토 후 pull-request를 받아주게끔 해야한다. <br/>
                       받아져야지 정상적으로 commit이 된다.
  
  * __README.md__ : 우리 프로젝트가 어떤 프로젝트인지 간략한 설명을 하는 곳
  
  * __Wiki__ : README.md와 같은 역할
  
  * [동기화]("./Git.md") <br/>
     
    GitHub Tutorial - Git에서 말했듯이, 작업 전 git pull 혹은 git clone을 해야한다. <br/>
    만일 작업이 끝났는데 작업한 코드가 진작에 Github에서 업데이트 된 코드인 상황을 방지하기 위해서다. <br/>
    처음 동기화 시킬 때는 git clone '원격저장소 주소'(실제로 ''는 없다.) <br/>
    그 후는 git pull '원격저장소 주소' 를 입력하면 된다. 이때 원격저장소의 주소를 origin으로 저장했으면 주소를 origin으로 대체해도 된다. <br/>
    pull과 clone의 큰 차이는, clone은 곧이곧대로 모든 파일을 다운받는 것이고, pull은 서버의 파일을 git과 비교하여 다운 받는 것이다. <br/>
    따라서 처음 한번만 clone을 하고 그 후에는 pull을 하는 것이다.
 

