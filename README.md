# DACON_Distribution
![20220524_114520](https://user-images.githubusercontent.com/84311270/169938520-1dc6a845-b06a-46e0-969b-70a3c11db93e.png)
제주시 내 택배 운송 데이터를 이용하여 운송량 예측 AI 개발

# Dataset
train_df.csv  
index : 인덱스  
송하인_격자공간고유번호  
수하인 격자공간고유번호  
택배_카테고리  
운송장_건수  

test_df.csv  
index : 인덱스  
 송하인_격자공간고유번호  
수하인 격자공간고유번호  
택배_카테고리  

sample_submission.csv  
index : 인덱스  
운송장_건수  

## Model
데이터에 대하여 One-hot Encoding을 진행하였고 Catboost 모델을 사용. Optuna를 사용하여 hyper-parameter 최적화 진행.

## Results
Public Score : 5.34231, Private Score : 9.02922로 최종 10등올 상위 1%로 대회를 마무리.
![20220524_114611](https://user-images.githubusercontent.com/84311270/169938892-f573b2fd-d955-4414-a4fe-7775afa2c1f3.png)

