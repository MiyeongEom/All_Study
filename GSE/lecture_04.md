## GSE 04
<br/>

#### 버전 관리 시스템(VCS)
* __변화를 시간에 따라 기록__
* 각 파일을 특정 시점으로 되돌리기 가능
* 시간에 따른 수정 내용 파악 가능
* 문제 원인 파악 가능
* 소스코드, 문서 등 모든 파일 형식의 데이터 대상
* -> 기본적인 VCS 이해 필수, SW개발에 있어 매우 중요  

#### 로컬 버전 관리 시스템 (Local VCS)  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/c5017954-93fe-44cc-b617-026c9840fc05)  
* 간단한 데이터 베이스
* 파일의 버전 정보 관리
* 한 사람이 관리
* ex) RCS(Revision Control System)  

#### 중앙집중식 버전 관리 시스템 (Central VCS)  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/ddf8f31b-4804-4d64-89a5-a7ce20f39780)  
* 협업을 위한 버전 관리
* 서버 존재
* 클라이언트 존재
* 서버 데이터 받아 사용
* ex) CVS(Concurrent Versions System), Subversion, Perforce  

#### CVCS의 핵심  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/0fb02634-2020-4d32-982c-dc55c0a7fa6b)  
* 장점 : 누가 무엇을 하는지 쉽게 판단 가능, 관리가 쉬움(서버 VCS 하나만 관리)
* 단점 : 서버 다운, 로컬 데이터의 스냅샷이 명확하지 않음 -> 복구 어려움  

#### 분산 버전 관리 시스템 (Distributed VCS)  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/a82b227a-df81-442c-beb8-2c32cfc9381c)  
* 협업을 위한 버전 관리
* 서버 존재
* 클라이언트 존재
* __서버의 모든 데이터 복제__
* ex) Git
* 특징 : 모든 데이터를 클라이언트에 복제, 서버 다운시 클라이언트 기반 복구 가능
* 장단점 : 사용해보고 알아보장  

#### Git 프로젝트 목표  
* 빠른 속도와 단순한 구조
* 비선형적인 개발 (수천 개의 동시 다발적의 브랜치)
* 완벽한 분산
* 대형 프로젝트에도 유용할 것  

#### Git VCS의 핵심  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/72fef5cc-6a6f-4a54-b768-64a8684367a1)  
* 모든 __데이터는 로컬 저장소__ 에 존재  
* 공유는 어떻게 ?  (핵심)
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/fb2716c7-b6e3-4d1c-9e28-b23bf1c6b6d8)  
* 작업 내용의 반영을 위한 로컬 저장소 -> 작업PC
* 작업 내용 공유를 위한 원격 저장소 -> 원격 PC

#### CVCS vs Git VCS  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/fae7e368-8b6b-490b-b117-191ee6e0aa17)  
![image](https://github.com/MiyeongEom/All_Study/assets/112458035/84f65197-197c-4583-a3ef-4c4f0244d09a)  

* Git VCS
  * 모든 데이터가 로컬 저장소에 저장
  * 원하는 버전을 아주 빠르게 얻을 수 있음 (스냅샷)
  * 서버와의 통신 적음
  * 서버 다운 시 작업 진행 및 복구 가능  
