# DL_Titanic disaster
- 타이타닉 생존율 딥러닝 이용하여 분석 및 성능 향상
- 프로젝트 기간

    > 2024.10.14 ~ 2024.10.17
    
</br></br>

## 1. Project Detail
- 모델 : 딥러닝 pytorch Neural Network 이용
- 독립변수 : 'Pclass', 'Sex', 'SibSp', 'Parch', 'Age'
- 종속변수 : 'Survived'

</br></br>

## 2. Data preprocessing 
- age 변수는 결측치가 많기 때문에 Name 변수에서 last name 추출하여 randomforestregressor 모델 이용하여 분석 후 결측치 채우기.
- n_estimator : 300

</br></br>


## 3. Data scaling 
- age 값은 StandardScaler 스케일러 이용하여 평균 0, 분산 1인 정규분포 갖도록 통일

</br></br>


## 4. Tuning
- epoch : 400
- batch size = 64

- input : 5 layer
- hidden : 6 layer
- output : 1 layer

</br></br>


## 5. Module
- ReLU 함수
- dropout 0.2
- return시 sigmoid 함수

</br></br>

## 6. Optimizer
- Adam
- learning rate = 0.001
- betas = (0.9, 0.999)
- eps = 1e-8
- weight decay = 0.001

</br></br>


## Output
Best score : 0.80143
