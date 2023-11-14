## Git 00
<br/>

#### Git 기초  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/256b5557-9c2f-4346-abf9-5954195357df)  
* 저장소 전부가 복제
* 문제 발생 시 복제물로 복구
* 최시 버전 끌어오는 것 (모든 데이터 백업 의미)
* 네트워크가 아닌, 해시(스냅샷) 포인터 형태로 관리하기에 여기저기 있는 정보를 바로 끌고 올 수 있음
* 깃에서는 스냅샷이라 하면 버전이라 생각해도 무방
* 대부분 __로컬__ 에서 실행됨 -> __네트워크 사용 최소화, 오프라인 상태에서도 작업 가능 (커밋 가능)__
* __무결성, 데이터 삭제 불가__
* 최대한 변화만을 저장하려고 함, 해시코드 -> 일대일 매핑 가능  
  
* 파일은 세 단계로 구성됨
  * Working Directory : 실제 모든 파일, 디렉토리 존재, 변경사항 추적 중
  * Staging Area : 변경 사항이 최종 커밋에 포함될 준비가 됨, 어떤 파일을 포함할지 선택 가능. 이 영역에 올라가면 다음 커밋에 포함될 변경사항으로 표시 됨
  * .git directory(Repository) : git저장소의 핵심, 모든 히스토리와 메타데이터 포함, 커밋로그/브랜치정보/원격저장소 주소 등, 로컬 저장소에 존재
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/c84b1c74-31bf-472e-b1cb-b4a9b07e4e83)  

* git init
  * .git 디렉토리가 생성됨
  * git clone은 다른 곳에서 git init으로 만들어진 repository 복제
* vim a.txt  //a, git add, gir commit -m "a"
  * commit : 버전을 만든다. 해당 버전에 대한 유일무이한 id 생성
  * vim : w(저장), q(나가기)
* 빨간색 표시 -> 날라갈 염려가 있어 손봐야 하는 부분
* 초록색 표시 -> 바뀌었는데 조금 안정화되었어  
  
#### Git  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/41777fbe-2c62-4fda-8d3d-a33d9858de2d)  
* untracked : 파일이 새로 등장함
* git .add -> 얘가 staged됨
* 커밋한 이후로 워킹과 깃 내용이 같다 -> unmodified (가장 안정화 됨)
* 근데 파일이 추가되거나 수정됨 -> 파일이 바뀜 -> 반영해야 돼(modified) -> .add(staged) -> commit(unmodified) -> 파일 삭제 (untracked)
