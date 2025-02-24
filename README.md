
# 자연어 처리란?

>**자연어 처리(NLP)는 머신러닝(Machine Learning)을 사용하여 텍스트의 구조와 의미를 파악하는 기술을 의미**

입력된 문장을 분석하여 다음에 오는 단어를 예측하거나 사람의 감정을 판별하는 것이 가능하고 더 나아가 문장을 구사하여 사람과 대화도 가능한 기술
*****
## 프로세스 순서

#### 1. 형태소 분석 (Morphoogical Analysis)
: 텍스트를 형태소 단위로 분할하여 각 형태소의 품사를 분석
- 문장을 단어 단위로 쪼개어 각 단어의 역할과 의미를 파악하는 것이 목표
#### 2. 구문 분석 (Syntax Analysis)
: 문장의 구조를 파악하여 단어들 간의 관계와 문장의 구조를 분석
- 문장을 문법적으로 분석하여 문장의 구조를 이해하고, 의미를 파악하는 것이 목표
#### 3. 의미 분석 (Semantic Analysis)
: 문장의 의미를 파악하기 위해 분석
- 각 단어들의 의미와 문맥을 고려하여 문장의 의미를 추론하고 해석하는 것이 목표
#### 4. 화용 분석 (Pragmatic Analysis)
: 문장의 맥락과 사용된 언어적 특징을 분석
- 문장에서 화자의 의도, 상황, 대화의 맥락 등을 파악하여 문장의 의미를 이해하는 것이 목표

## 전처리 과정

>**모델의 성능을 향상 시키기 위해 말뭉치(Corpus)를 정제 후 컴퓨터가 처리 가능하도록 벡터화를 수행하는 과정**

- **문장 분리** : 입력된 텍스트를 문장 단위로 분리
- **토큰화(Tokenization)** : 문장을 단어 혹은, 구문 단위로 분리
- **정제, 정규화(Normalization)** : 대/소문자나 같은 의미를 가진 단어를 하나로 통일
- **불용어(Stopword) 제거** : 자주 등장하지만 의미를 가지지 않는 단어를 제거
- **표제어 추출 (Lemmatization) 또는 어간 추출 (Stemming)** : 단어를 기본 형태로 변환
- **Bag of Words (BoW)** : 단어의 순서를 배제하고 빈도수 기반으로 수치화하여 집합 형태로 표현
- **TF-IDF (Term Frequency-Inverse Document Frequency)** : 단어의 중요도를 계산하여 문서를 벡터화
- **Word Embeddings** : 모델 학습을 위해 단어를 고정 크기의 벡터로 변환하는 과정
- **문장 구문 분석 (Syntax Parsing)** : 문장의 구조를 분석하여 문법적 구조를 추출

## 사용 분야

>**NLP(Natural Language Processing)** 을 통해 컴퓨터가 문장의 의미를 분석하는 것이 가능해지면서 감정 분석, 기계 번역, 내용 요약, 질의 응답 시스템 등 다양한 분야에서 활용이 가능

- **기계 번역** : 모델이 입력된 단어들의 의미를 정확히 파악하고 가장 적합한 단어를 선정하여 다른 언어로 번역해주는 기술로 `트랜스포머(Transformer)` 를 통해 문장 구사력을 높여 자연스러운 번역을 구현하는 것도 가능
- **추천 시스템** : 모델이 사용자의 데이터를 학습하여 각각의 리뷰나 평가와 같은 텍스트 데이터에서 감정을 파악함으로 사용자의 선호도나 관심사를 도출, 이에 기반하여 사용자의 요구에 맞는 적절한 답변을 생성하거나 추천하는 것이 가능
- **문장 요약** : 입력된 문장에서 문맥의 흐름과 중요도가 높은 키워드를 도출하여 해당 키워드를 위주로 문장을 재구성하는 것이 가능

이외에 텍스트 분류나 질의 응답과 같은 다양한 분야에서도 활용이 가능하며, 대표적인 기술이 OpenAI의 [ChatGPT](https://chat.openai.com/ ChatGPT)나 Microsoft의 [MS Copilot](https://copilot.microsoft.com/ MS Copilot) 등이 존재
