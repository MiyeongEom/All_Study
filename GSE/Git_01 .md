## Git 01
<br/>

#### 파일 상태 확인 (untracked, modified, staged)
* git status
* git status -s : 단축되어 정보 표시

#### 파일 새로 추적하기
* 파일 추가 -> git status : 빨간색
* git add (file name) -> repository에 올리기 전(커밋 전) : new file: 연두색
* commit -> clean  

#### staged(올려진)와 unstaged(방금 막 작업) 상태의 변경 내용 보기
* git diff (working directory, staging area 비교)
* git diff -staged|cached (staging area, .git repository 비교)  

#### 파일 삭제
* gir rm (file name)  : stage와 working 양측에서 모두 삭제
* 아래의 동작과 같음
  * rm (file name)
  * git add file name
* stage 된 파일만 삭제하려면? : gir rm -cached (file name)  
  
#### 파일 이름 변경
* git mv (file name) (new file name)
* 아래의 동작과 같음
  * mv (file name) (new file name)
  * git rm (file name)
  * git add (new file name)  
 
#### 커밋 히스토리 조회
* git log
