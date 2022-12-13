# Clothing_Recommend_Prediction
의류 판매 상품 리뷰 분석을 통한 상품 추천 여부 예측
## 프로젝트 목차

1. **데이터 읽기:** 이커머스 데이터를 불러오고 Dataframe 구조를 확인


2. **데이터 정제:** 비어 있는 데이터 또는 쓸모 없는 데이터를 삭제<br>
    2.1. 결측값 확인<br>
    2.2. 결측값 처리<br>


3. **데이터 시각화:** 변수 시각화를 통하여 분포 파악<br>
    3.1. `Title` word cloud<br>
    3.2. `Review Text` word cloud<br>
    3.3. `Recommended IND` 시각화<br>


4. **데이터 전 처리:** 머신러닝 모델에 필요한 입력값 형식으로 데이터 처리<br>
    4.1. 자연어 전 처리 - Tfidf<br>
    4.2. 학습, 테스트 데이터 분리<br>


5. **머신러닝 모델 학습:** 분류 모델을 사용하여 학습 수행<br>
    5.1. 기본 분류 모델 학습 - 의사결정나무<br>
    5.2. 다양한 분류 모델 학습<br>


6. **평가 및 예측:** 학습된 모델을 바탕으로 평가 및 예측 수행<br>
    6.1. Confusion Matrix<br>
    6.2. Precision & Recall<br>
    6.3. 테스트 데이터의 예측값 출력


## 데이터 출처 
- https://www.kaggle.com/nicapotato/womens-ecommerce-clothing-reviews


## 프로젝트 개요

언택트 시대가 다가오면서 의류, 식료품, 전자제품 등 다양한 상품을 인터넷을 통하여 거래하게 되었습니다. 수많은 상품이 인터넷상에서 전시되어 있지만, 실제로 사용한 상품이 아니라면 나에게 맞는 상품인지를 알기 쉽지 않습니다. 이러한 단점을 극복하기 위하여 수많은 이커머스 웹사이트에서는 상품 리뷰 글을 남길 수 있도록 하고 최대한 많은 리뷰가 나올 수 있도록 장려하고 있습니다. 소비자는 이러한 리뷰를 통하여 실제 후기와 상품 정보에서 미쳐 파악하지 못한 정보들을 얻을 수 있으며, 긍정적인 리뷰가 많은 상품에 대해서는 신뢰도 또한 가질 수 있게 됩니다. 판매자 입장에서도 리뷰가 많은 상품을 마케팅 요소로 사용할 수 있으며, 소비자의 의견을 들을 수 있는 장점이 있습니다. 따라서 이커머스에서는 리뷰는 상품을 구매하는 데 있어서 매우 중요한 특성 데이터로서 가치가 있습니다.

이번 프로젝트에서는 Kaggle에서 제공하는 여성 의류 이커머스 데이터를 바탕으로 상품 추천 여부를 예측해보는 분류 모델을 구현합니다. 이를 통하여 새로운 리뷰와 여성 의류 정보를 받았을 때, 해당 상품을 추천하는지를 예측할 수 있습니다. 이를 활용하면 상품 추천 여부가 없는 상품들에 대해서도 리뷰와 의류 정보를 바탕으로 상품 추천 여부를 예측할 수 있으며, 이는 상품의 중요한 지표로서 다시 활용될 수 있습니다. 


- https://2022aionline.elice.io/courses/28467/lectures/216166/materials/1/
