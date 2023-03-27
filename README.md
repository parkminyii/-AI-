# 감정 인식 기반 공감 AI 챗봇

## 기획의도와 목표
    챗봇 모델의 공감성을 강화하기 위해 트랜스포머 기반의 다중 분류 모델로 구현한 감정 분류 매커니즘을 추가하고 
    텍스트와 함께 사용자의 감정을 표현할 수 있는 이미지를 함께 답변함으로써 공감능력을 강화하고 재미를 더해 사용자의 만족도를 높인다.

## 시스템 흐름도
<img width="80%" src="https://user-images.githubusercontent.com/72790897/227712123-d27a035a-e1cd-4be2-84da-9c2b3405a36b.png"/>
<img width="80%" src="https://user-images.githubusercontent.com/72790897/227712131-a80f4f9c-4e46-423b-adc3-77e602b4fa22.png"/>

## Data
### reference
    - 송영숙님의 Chatbot_data
    - https://github.com/songys/Chatbot_data
    - 감성 대화 말뭉치 
    - https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=86
    - 감성 및 발화 스타일별 음성합성 데이터 (대화체-감정분류 데이터만 사용)
    - https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100&aihubDataSe=realm&dataSetSn=466 
    - Smilegate AI에서 공개하는 한국어 문체 스타일 변환 "SmileStyle" 데이터셋
    -https://github.com/smilegate-ai/korean_smile_style_dataset
    - FER-2013 (Face Emotion)
    - https://www.kaggle.com/datasets/ananthu017/emotion-detection-fer
    - celebA
    - http://mmlab.ie.cuhk.edu.hk/projects/CelebA.html


## Models
    모델학습/ 참조

### reference
    - kobert
    - https://hoit1302.tistory.com/159
    - kobart
    - https://heegyukim.medium.com/korean-smilestyle-dataset%EC%9C%BC%EB%A1%9C-%EB%AC%B8%EC%B2%B4-%EC%8A%A4%ED%83%80%EC%9D%BC%EC%9D%84-%EB%B0%94%EA%BE%B8%EB%8A%94-%EB%AA%A8%EB%8D%B8-%EB%A7%8C%EB%93%A4%EC%96%B4%EB%B3%B4%EA%B8%B0-d15d32a2c303

## 구현한 코드
    시스템 기능/전체시스템구현_tf.ipynb

## 차후 목표
    - Colab 기본을 개발환경으로 이용 ->  RAM과 런타임 시간 한계
    - 속도 등 성능 향상을 위한 개선 필요
    - 챗봇 DB, 말투 DB를 더 추가하고 최적의 파라미터 값을 더 찾아본다면 목적에 알맞게 성능을 높일 수 있을 것이라 기대함
    - 더 나은 환경이 주어진다면 챗봇은 gpt3, 감정분류모델은 koelectra 등 더 좋은 모델 학습을 해보고 싶음
    - 최종적으로 서비스화한다면 앱을 생각함



