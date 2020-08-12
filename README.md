# SCC_Project 2.
##### 2020 Summer Coding Camp - Project #2 (Prof. KIM HJ)
###### 21600402 Ahn SuHyun


## Task : Graphic Editor 
### Time Period : 4 days 


![image](https://user-images.githubusercontent.com/64300241/90040630-25f9f500-dd03-11ea-9468-284b57a4d35f.png)




#### 기능 구현
1. 펜 (자유곡선), 지우개(비트단위 자유곡선), 직선도형, 타원형, 삼각형, 직사각형, 마름모, 평행사변형, 오각형, 육각별
2. 상단라벨에 현재 타입 알아 볼 있게 둠 
3. 드래그 하는 중에는 반투명 + 하이라이터를 통해 도형 예상 및 유도 제공 
4. 선색과 내부 색 분리 구현
5. Undo / Redo : 모든 그림에 대해 적용 가능, 작업 이상의 Undo / Redo 입력을 해도 안정성 확보 
6. Select 모드에서 선택할 있는 그림은 마우스 커서를 변경하여 알림, 그림 더블 선택으로 '선택' 및 선택한 오브제 이동 
7. 지우개 사용시 마우스 커서를 가리고 지우개 포인터 제공, 지워지는 실루엣 트레이싱을 제공 
8. 편집 -> 클리어를 통해 화면에 있는 요소를 전체 날릴 수 있음, undo redo 가능 
9. 파일 -> 새로만들기를 통해 모든 버퍼를 비우고 처음부터 다시 시작할 수 있음 
10. 배경색 변경 -> 배경색과 기본 지우개 색 연동 
11. 저장 및 불러오기 가능, 작업 순서를 기억해서 불러온 파일도 undo redo 가능 

##### 버그 및 구현 못한 거 
1. 자유곡선 선택 및 이동시 불안정성이 아직 있음 
2. 위치를 이동하면 버퍼의 저장된 정보 자체르 수정하는 것이기 때문에 undo를 해 이동전 위치가 아니고 제일 마지막에 그렸더 도형이 지워짐
3. 편집 -> 클리어를 통해서 저장하거나 도중에 배경색을 변경하면 논리가 아직(어렵지 않음) 모자라서 연동이 안될 수 있음 
4. 변경한 배경색은 저장이 되지 않음 (저장하는 필드를 구현 안함 ) 

## 배운점 
1. 싱글 톤으로 유기적인 프로그래밍 
2. Object 단위 Stream & Serializable 
3. Referenece Type -> Deep Copy
