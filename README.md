# kesla_project ( 현재 업데이트 중입니다. )
[2020.03~] 졸업프로젝트 - 붕괴 위기가 있는 건물에서의 조난자 탐색 로봇

# 1. summary
붕괴 위기가 있는 건물에서 사람이 직접 들어가는 것은 위험부담이 매우 크다.  
이를 해결하기 위해 사람을 인식할 수 있는 로봇을 대신 진입시켜  
건물 내를 꼼꼼히 탐색하고 조난자가 있는 위치를 맵에 표시하여  
인명 구조 작업을 위한 정보 습득을 위해 사용한다.  

# 2. 상황 설정
1. lane tracking : 도로가 건물까지 이어져 있고 터틀봇은 도로를 따라 건물까지 도달한다.
2. exploration : 건물에 진입해 건물의 map 정보를 모두 얻을 수 있을 때까지 탐색한다.
3. recognition : 사람을 인식해 map에 표시한다.
4. navigation : 2~3 과정이 모두 끝나면 건물을 탈출한다.

# 3. 하드웨어 setting
* 로봇 : turtlebot3 burger
  * computing resource : nvidia jetson nano (터틀봇에 장착)
  * camera : 라즈베리파이용 webcam
* commander 
  * computing resource : notebook
  
# 4. 구조 
현재 필요한 mode를 받아와 해당 mode에 맞는 프로그램(Ros 패키지)을 실행시킵니다.
<img src="./image01.png" width=800px>
