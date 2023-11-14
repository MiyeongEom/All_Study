## Git 02
<br/>

#### Git branch
* 모든 VCS는 브랜치를 지원함
* 원래 코드를 유지하며 독리적으로 개발 진행 시 필요
* git의 최고 장점 : 매우 가벼운 브랜치  
  
* git은 commit 이후 아래와 같은 데이터를 저장, 커밋 아이디는 중복되지 않으며, 이 아이디를 파고 들어가면 워킹 디렉토리에 있는 모든 내용 알 수 있음
  * blog : Git 이 저장하는 파일 형식을 칭하는 용어  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/49441384-8d31-4087-bbf8-a7835dc7a2cc)  
  
* commit이 될 때마다 새로운 커밋 아이디 생성, 이전 아이디를 parent로 저장, 두 번째 사진 -> 간략히 표현  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/c4911649-5b43-471f-b586-891a663e7861)  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/ccfc916a-645f-4c1e-8ee3-43a2f9579050)  

#### Branch
* 가지라는 의미.
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/fa99567b-924a-44fd-ac77-b769b6dd92e0)  
* commit 할 떄마다 __해당 id <- master <- head__
* head는 master라는 branch를 가르키며, 이가 아이디를 이동해 다님
* head가 가리키는 id가 변경되면 해당 id가 가진 정보를 기반으로 Working Directory 를 구축 -> 버전 이동을 의미함  

