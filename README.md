# 데이콘 대회 정리!
## 이번에 데이콘 2022 관광데이터 AI 경진대회에 나갔습니다.
### https://dacon.io/competitions/official/235978/leaderboard
### 데이터는 자연어와 이미지가 있었습니다.  그래서 저희팀은 자연어 모델과 이미지 모델로 2개의 조로 나눠 사전학습모델을 이용하여 모델링을 하고, 앙상블을 계획했습니다.
### 저는 자연어 사전학습모델인 bert를 이용하여 모델을 구축하였습니다. 저는 데이터를 보고 제일 처음한 것이 데이터의 노이즈를 제거하는 것을 하였습니다. 데이터에는 HTML태그와 한자 그리고 특수문자가 있어서 제거하였습니다. 모델을 구축하고, 전처리도 해보고, Kiwi를 이용하여 형태소도 분류해봤으나 성능이 오히려 떨어졌습니다. 그래서 어쩔 수 없이 전처리보다 모델링에 신경쓰는 것을 주로 하였습니다.
### 모델링에서 batch size와 lr를 줄이는 것이 성능에서 효과를 보였고, Adam에서 NAdam을 사용하는 것이 성능이 좋았습니다.
### 이번 프로젝트를 하면서 아쉬웠던 것은 전처리였습니다. 대회 마감 2일을 앞두고, 전처리를 하고 군집화를 하여 보는 방법이 있었는데 시간이 없어서 못한 것과 이미지 모델이 생각보다 성능이 많이 안나와서 앙상블을 못한 것이 아쉬웠습니다.
### 전처리에 대해 아직 공부가 많이 부족한 것 같아 좀 더 공부를 해야할 것 같고, 전처리에 대한 검증 또한 많이 해봐야 할 것 같습니다!
