# 👨‍🍳 LDA를 활용한 부정서비스 리뷰 분석

  맛집 추천 사이트인 다이닝 코드에서 리뷰데이터와 유저들이 평가한 평점데이터를 활용하여,
  
  "서비스" 항목에서 부정평가 ( 3이하 )를 받은 리뷰를 LDA를 통하여 분석하였습니다.
  
  자세한 내용은 저희 논문 https://www.dbpia.co.kr/journal/articleDetail?nodeId=NODE11229799 를 참조해 주세요.


# Data


<p align='center'>
    <img src='https://github.com/seunghyeon98/LDA-/assets/111716640/0ebde4d9-3979-4aba-85f5-4723a0fa7b88' width='300'>
</p>
 
연구를 목적으로 맛집 추천 사이트인 "다이닝코드" 에서 셀레니움을 통하여 크롤링 하였으며,
리뷰데이터를 전처리한 과정은 사진과 같습니다.

          
# Method

<p align='center'>
  <img src ='https://github.com/seunghyeon98/LDA-/assets/111716640/76dd7bc5-f83a-4025-9839-c5582bd4e9a8' width='800'>
</p>

서비스 부분 항목에서 3점 이하를 받은 리뷰를 서비스에 대한 부정적인 평가를 하였다고 가정하여 클러스터 분석을 하기위해 Topic Modeling 기법중 하나인 LDA를 사용하였습니다.


# Analysis & Result

<div align="center">
  <div style="display: flex; flex-direction: column;">
    <div style="text-align: center;">
      <img src="https://github.com/seunghyeon98/LDA-/assets/111716640/ff66560b-8053-4f58-9b45-9bb7ca3b3303" alt="이미지 제목" width="400">
      <p>[무형으로분리된 그룹]</p>
    </div>
    <div style="text-align: center;">
      <img src="https://github.com/seunghyeon98/LDA-/assets/111716640/9a7835aa-1ce4-450b-bc7e-2341fbd9a8e5" alt="이미지 제목" width="400">
      <p>[유형으로분리된 그룹]</p>
    </div>
  </div>
</div>



<p align='center'>
  <img src='https://github.com/seunghyeon98/LDA-/assets/111716640/a32e2970-d59a-426f-b3bf-1dd1e639b472'>
</p>

LDA의 결과를 통해 나온 각 단어를 종합하여 서비스에 대한 분류를 2가지 측면으로 분류하였습니다.

유형적인 분류는 "장소","공간"을 나타내고 있는 그룹,
무형적인 분류는 "사람","감정"을 나타내는 그룹으로 분류하여 종합하였습니다.

