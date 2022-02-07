# QA Model Project

한국어 지문에 따라 질문에 맞는 답을 생성하는 QA 프로젝트입니다.

## 목적

Bert 모델을 활용하여 기존 학습 모델의 성능을 개선합니다.

---

### Requirement

- torch 1.9.1
- transformers 4.11.3
- tensorboard
- konlpy
- tweepy<4.0.0

### Preprocess

- 데이터 셋의 구조
![image](https://user-images.githubusercontent.com/92852871/152847741-036cbd22-fe90-4f96-a0ed-4ebc5cb0ef8a.png)

- knolpy의 mecab을 활용하여 형태소를 분석

### Train

- BertForQuestionAnwering 사용
- optimizer : AdamW 사용
- SummaryWriter 사용 - epoch별 모델 eval_loss, train_loss 확인

### issue

- 과적합 발생
- 편집거리 측정으로 인한 후처리 필요

