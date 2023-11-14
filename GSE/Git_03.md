## Git 03
<br/>

#### branch 생성  
* __git branch (branchName)__  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/38c336b4-b424-4c6b-8e67-67c03d59420d)  
* 브랜치 생성 바로 직후 : HEAD는 기존의 master 브랜치의 fd47dle
* 브랜치를 dev 생성 -> 단지 fd47dle를 가지고 있음, 생성 순간 master의 브랜치 정보를 그대로 복사
* 다른 브랜치를 작업하려면 head의 이동이 필요함.  
  
#### branch 이동
* __git checkout (branchName)__
* 문제가 없다면 HEAD 가 dev 브랜치의 마지막 commit id인 fd47dle를 포인팅 함
* git은 이동 명령 입력 순간 아래와 같은 사항 체크
  * staging area가 비어있는가?
  * working directory 내용에 변화가 있는가?
 
#### staging area가 비어있지 않은 경우
* Staging area엔 브랜치 정보가 존재 하지 않음 -> 문제가 있다면 브랜치 이동을 막아야 함
* staging에 있는 경우 checkout해도 오류가 존재X
* 새로운 파일을 생성하고 add 하고 checkout 하면 그 파일이 딸려서 온다.  (commit 기록이 없음, 데이터 손실 최소화)
* 그러나 다시 돌아가서 파일을 변경하고 add/commit하지 않고 master로 돌아오려고 하면 오류가 난다 (기존 파일을 덮어쓸 수도 있기 떄문에)
* commit 해라  

* git add 명령어를 사용하여 작업 디렉토리에 있는 변경된 파일을 스테이징 영역에 추가하면, 해당 파일은 스테이징 영역에 존재함
* 이미 커밋한 파일을 수정하는 경우 또한 스테이징 영역에 존재.
* 이전 커밋에서 추적되고 있는 파일을 수정하면, 해당 파일의 변경사항이 스테이징 영역에 추가되어야 새로운 변경사항이 기록됨

#### Working directory 내용에 변화가 있을 경우
* HEAD 정보를 기반으로 판단함.
* 헤드 정보와 옮겨 가고자 하는 브랜치의 죄종 COMMIT ID기준으로 이동 가능 여부 판단  
  
