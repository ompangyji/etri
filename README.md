
# 제지 공정 시스템 에너지 절감을 위한 데이터 분류 및 특성 연구
<p align="center">
<img src = "C:\Users\hnoo0\etri\assets\image1.png" width="700" height="400">
</p>

# 1. 연구 목적
<p align="center">
<img src = "C:\Users\hnoo0\etri\assets\image2.png" width="700" height="200">
</p>

- 생산 가동(연속공정) 중 지절이 발생하면 제지공정의 안정화를 위해 진단 및 유지 관리 시간이 생기게 되고 펄프, 전력 등 의미없는 자원 소모
- 지절 발생에 대한 영향인자를 파악하고자 함

# 2. 상관성 분석

- 스피어만 상관계수
  비선형 관계의 연관성을 파악
<p align="center">
<img src = "C:\Users\hnoo0\etri\assets\image3.png" width="600" height="400">
<img src = "C:\Users\hnoo0\etri\assets\image4.png" width="600" height="300">
</p>

- 실린더, 드라이, 지종, 스팀 압력, 수분량, 회분량, 공정 에너지 전력에 연관된 태그가 지절과의 상관성이 있다는 것을 확인

# 3. SVM 분류 모델링

- 독립 변수 : 지종
- 종속 변수 : 평량, 지절유무, 상관성 분석을 통해 추출된 요인

<p align="center">
<img src = "C:\Users\hnoo0\etri\assets\image5.png" width="600" height="450">
</p>

- Accuracy : 0.98

생산하는 지종을 특정할 수 있었고 지종은 지절 현상과 관계성이 있다는 것을 확인


# 4. t-SNE 차원 축소를 활용한 시각화

<p align="center">
<img src = "C:\Users\hnoo0\etri\assets\image6.png" width="65" height="500">
<img src = "C:\Users\hnoo0\etri\assets\image7.png" width="450" height="450">
</p>

- 그룹1(고평량)
  #0, #3, #7, #8, #9, #16
- 그룹2(저평량)
  #1, #2, #3, #5, #6, #10, #11,  #12,  #14
- 그룹3(중평량)
  #13, #15

:point_right: [노션](https://www.notion.so/01c9f82a89e6456cab424921452a8df1) 자세한 내용
