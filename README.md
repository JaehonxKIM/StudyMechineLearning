# StudyMechineLearning

### 1일차
  - 머신러닝의 개요(구글 collab사용)

### 2일차 
  - 머신러닝을 활용한 데이터 분석 플로우

### 3일차
  ### 개요
    - 플라스크 기반 웹서비스
    - 머신러닝 모델을 적용한 서비스
    - 파파고 유사 형태 제공

  ### 사전지식
    - 웹 분야중 클라이언트 구성은 3개로 구성
        - html5 : 뼈대, 콘텐츠
        - css3  : 디자인, 레이아웃, 데코레이터, 반응형
        - javascript : 이벤트, ajax(비동기 네트워크), 화면조작(동적 화면 구성), 이 파트는 써드파트 모듈이 다양하게 존재함(jQuery, bootstrap,..)
    - 클라이언트가 서버로 데이터를 전송하는 방법
        - form 전송 : 주소창 옆에 새로고침 아이콘이 x로
            변경된다(아주 짧게). 그리고 화면이 새로고침 된다
        - ajax 전송 : 화면 변화 없다. 응답 결과로 변경할수는 있지만 페이지는 고정되어 있다
            - 파파고와 유사해야 하므로, 이 방식으로 진행

  ### 프로젝트 구조
    /
    L templates  : *.html이 위치하고, 화면 랜더링시 사용
        L index.html
    L run.py     : 엔트리 포인트
    
    L readme.md  : 코멘트, 설명
### 4일차
  - 모듈 삽입

### 5일차
  - 성능 평가
    - iris 데이터를 활용해서 어느 알고리즘이 높은 정확도를 보여주는지 평가
  - 교차 검증
    - breast_cancer 데이터를 활용해서 독립변수와 종속변수의 shape을 알아보고 학습시키고 성능평가
    - 파이프라인 구축 과정 초반까지
### 6일차 
  - 하이퍼파라미터 튜닝
  - 최적의 파라미터 값 구하기
  - 파이프라인 구성 
  - 의사결정트리의 개요
    - 결정트리 의사결정 분기과정 시각화
    - 과적합 처리
    - 등고선 plot 그리기 기본

### 7일차 
  - 과적합 처리
  - 앙상블 
    - 랜덤포레스트
  - 보팅
    - 소프트보팅 : 다 더해서 평균
    - 하드보팅 : 다수결
  - 부트 스트래핑
    - 성능평가
    - 시각화
  - 부스팅
    - AdaBoost
    - GBM
    - XGBoost
  - 도구 관련 파라미터
    - 평가도구
      - rmse(root mean square error) : 정답과 예측 사이의 오차율 -> 작을수록 정확도가 높다
      - mse(mean square error) : 평균 제곱근 오차
      - mae(mean absolute error) : 평균 절대값 오차 -> 분류쪽에 활용
      - logloss : 손실에 로그처리
      - error
      - merror
      - mlogloss
      - auc
  - 머신러닝 과정(sklearn) -> 사이킷런 스타일로 Wrapping된 클래스 생성 -> fit() -> predict() -> 평가도구를 활용하여 판단

### 8일차
  - 스태킹(Stacking) : 
    - 원리
      - 여러 모델의 예측결과를 기반으로, 이 정보를 메타정보로 구축, 이를 이용해서 다시 학습 후 예측 수행
      - 모델은 2단계에 걸쳐서 생성
        - 예측결과가 데이터가 되는 구조
    - 정리
      - 1차 모델: 원본 데이터를 이용하여, 여러개의 알고리즘을 활용(서로다른)
      - 2차 모델 : 예측 결과를 데이터로 활용하여서 학습후 예측 
  - SVM
    - 가장 넢은 여백을 가지게끔, 클래스로 구분할 수 있게 경계선을 찾는다
    - 2개의 클래스를 확실하게 분류할 수 없다면, 가능한 최적의 경계선을 찾는다
    - 이미지 분류에서 많이 사용(전통적)
  - KNN 
    - 클러스터링에서 많이 사용  
  - CLUSTERING
    - 알고리즘을 활용하여 무리(군집)를 만들어내어 새로운 특징점을 혹은 분류라는 지점을 생성하는 기법
                 

