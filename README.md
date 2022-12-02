# DACON--AI-
데이콘 2022 관광데이터 AI 경진대회 (알고리즘 ,비전, 언어, 분류, Weighted f1 score)

### [2022 관광데이터 AI 경진대회(https://dacon.io/competitions/official/235978/overview/description)

## 첫 대회!!###
- 4명이서 팀을 구성했다.
- 주어진 데이터가 자연어와 이미지가 있어서 사전학습모델로 학습을 진행했다.
- 처음엔 자연어 먼저 사전학습모델이 아닌  CNN모델로 학습을 해보고 그 다음엔 이미지 사전학습모델인 resnet50으로 같이 돌려보았다.
- 이미지를 합치면 성능이 잘 나오줄 알았는데 생각보다 이미지가 성능에 크게 영향을 주지않고 오히려 더 떨어지기도 했다. 그래서 과감히 이미지를 버리고 자연어 위주로 사전학습모델로 학습을 했다.
- 사전학습모델중에서도 허깅페이스에 있는 bert모델을 사옹했다.
- 처음에 품사 태깅을 하고 데이터에 cat1,cat2,cat3의 각각 가중치를 임의로 설정했다. 데이터가 너무 커서
batch_size를 4로 설정하였고 optimizer 를 Adam으로 설정해 모델 학습을 했다.
- 그리고 마지막으로 각자 잘나온 모델들로 앙상블을 했다.


+ 첫 대회지만 나쁘지 않은 결과라고 생각한다.

![데이콘 순위](https://user-images.githubusercontent.com/80369260/198971282-71d5348a-ae5a-4f95-b244-00f5e937a0a6.jpg)

### 데이콘 차트
![데이콘 차트](https://user-images.githubusercontent.com/80369260/198971307-f4d43f7e-edce-4fcc-88a0-4f4b6bf137de.jpg)
