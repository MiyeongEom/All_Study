# L  
  
* LNK1168: 쓰기용으로 열 수 없습니다 (2023. 10. 24)
  * 파일이 사용 중이고 파일 핸들이 다른 프로세스에 의해 잠겨 있거나, 파일 또는 파일이 있는 디렉터리나 네트워크 공유에 대해 쓰기 권한 없음.
  * 이미 파일이 돌아가는 중인가 봄...
  * cmd -> __tasklist__ -> my .exe file searching -> check prcess id number -> __taskkill /f /pid (number)__  
