# 2.-AI-Goorm-QA-model

한국어 지문을 보고 질문에 맞는 답을 생성하는 프로젝트

이슈 : 기존의 train data는 과적합 발생 -> AIHub의 데이터 활용 / KoBert와 같은 pretrained 모델 사용

Tokenizer같은 경우 pretrained된 Tokenizer를 써야 함. pretrained 모델을 쓰기 위해서는
여기에 최적화된 토큰을 찾아 적합한 코드를 작성해야 함. KoBert의 토큰들의 길이는 대부분 512일것이고 1024 드물것
대부분의 콘텍스트의 길이가 512를 넘어가므로 어떻게 콘텍스트 길이를 늘릴 것인가에 대한 고민 필요
