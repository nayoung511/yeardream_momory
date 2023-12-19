# 이어드림 스타트업 연계프로젝트
(보안 상의 이유로 기업에서 제공받은 코드는 포함하지 않았습니다.)

---

## 프로젝트 상세 내용
**프로젝트 명:** 이어드림 스타트업 연계 프로젝트

**프로젝트 목적:** <기록을 통한 심리적 영향을 주는 객체 파악>
모모리는 사용자가 일상을 텍스트로 기록하고 감정을 체크할 수 있는 감정 기록 앱입니다. 주기적인 기록을 통해 사용자의 감정 패턴, 심리 상태, 인지 편향 등을 기록하고 분석합니다. 이 프로젝트를 통해 사용자의 기록을 NLP기술을 활용하여 분석하여 긍부정 영향을 끼치는 객체를 파악하고자 합니다.

**기간:** 2023.11.08 ~ 2023.12.15

**프로젝트 유형:** NLP, 딥러닝

**주요 기술 스택:** BERT

- 자연어 처리 (NLP):
	- 형태소 분석기: Hannanum
    - 개체명 추출 NER: xlm-roberta-large-finetuned-conll03-english, Leo97/KoELECTRA-small-v3-modu-ne
    - intfloat/multilingual-e5-base
    - 감정 추출: DanGam ()


**주요 역할 및 책임:**
[프로젝트에서 맡은 주요 역할과 수행한 책임]

---

## 주요 기술 스택

### 자연어 처리 (NLP)

#### 형태소 분석기: Hannanum
Hannanum은 한글 형태소 분석을 수행하는 도구로, 한국어 텍스트를 형태소 단위로 나누어주어 문장의 구조를 분석하는 데 사용됩니다. 프로젝트에서는 사용자가 입력한 텍스트를 형태소 단위로 분석하여 감정을 추출하는 데 활용되었습니다.

#### 개체명 추출 (NER)
- **xlm-roberta-large-finetuned-conll03-english:** 다국어로 학습된 RoBERTa 모델을 기반으로 한 개체명 인식 (NER) 모델입니다. 다양한 언어의 텍스트에서 중요한 개체를 추출하는 데 사용되었습니다.
- **Leo97/KoELECTRA-small-v3-modu-ne:** 한국어 텍스트에서 명사와 명사구 등의 개체를 추출하는 모델로 사용되었습니다.
- **intfloat/multilingual-e5-base:** 다국어로 학습된 BERT 모델을 기반으로 한 개체명 인식 모델입니다. 다양한 언어에서의 NER 작업에 적용되었습니다.

#### 감정 추출: DanGam
DanGam은 한국어 텍스트에서 감정을 추출하는 딥러닝 기반의 모델입니다. 사용자가 입력한 텍스트에서 긍정, 부정 등의 감정을 식별하고 분석하는 데 사용되었습니다.

### 딥러닝

#### 모델: BERT
BERT는 언어 이해를 위한 사전 훈련을 받은 모델로, 프로젝트에서는 자연어 처리 작업에서 활용되었습니다. 주로 문장의 문맥을 파악하여 텍스트 데이터의 의미를 이해하는 데에 사용되었습니다.

---
## 프로젝트 구조
![프로젝트 FlowDiagram](https://private-user-images.githubusercontent.com/44768141/291494788-2a8dfbd4-3ce7-4a0a-bf74-c07daab3b9e8.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTEiLCJleHAiOjE3MDI5NjcyODUsIm5iZiI6MTcwMjk2Njk4NSwicGF0aCI6Ii80NDc2ODE0MS8yOTE0OTQ3ODgtMmE4ZGZiZDQtM2NlNy00YTBhLWJmNzQtYzA3ZGFhYjNiOWU4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFJV05KWUFYNENTVkVINTNBJTJGMjAyMzEyMTklMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjMxMjE5VDA2MjMwNVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWY1MTM2YTljZTg1ZGNjNzFkNmZiYmYyNjdlOGYwNzIyZjA4MmE4NTJkYTg3ZjQxMmEzOTY2NjA5Y2E4MTkyMjEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.i2ZbgTZcnRJUdz4hyesROSlWwc8LCznfWq6JIcaJe28)
