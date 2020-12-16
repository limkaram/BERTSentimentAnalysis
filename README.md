# NLP Sentiment Analysis project

### 1. 실행 환경
- <b> 코드환경<br>
<t> Google Colab Pro(GPU)<br>
<t> Huggingface Transformers PLM(Pretrained Language Model) 활용
- <b>버전<br>
pytorch == 1.7.0<br>
transformers == 4.0.1<br>

<br>

### 2. NSMC 네이버 영화 리뷰 데이터 감정 분석

 - 코드 :  KoELECTRA_nsmc_sentiment_analysis.ipynb
 - 활용모델 : KoELECTRA-Base-v3 Discriminator

|                   |               | Layers | Embedding Size | Hidden Size | # heads |
| ----------------- | ------------: | -----: | -------------: | ----------: | ------: |
| `KoELECTRA-Base`  | Discriminator |     12 |            768 |         768 |      12 |


- <b>실행 방법 : 모든 셀 실행<br>


- <b>데이터 출처</b>  
<t>[Naver sentiment movie corpus v1.0](https://github.com/e9t/nsmc.git)


- <b>참고문헌 및 코드</b>    
 <t>[1. BERT로 네이버 영화 리뷰데이터 분류하기](http://yonghee.io/bert_binary_classification_naver/)<br>
 <t>[2. monologg/KoELECTRA Gitgub](https://github.com/monologg/KoELECTRA)<br>
 <t>[3. BERT에 대해 쉽게 알아보기](https://ebbnflow.tistory.com/151)<br>
 <t>[4. BERT 톺아보기](http://docs.likejazz.com/bert/)<br>
<br>


### 2. Friends 영화 대본 데이터 감정 분석

 - 코드 :  BERT_friends_sentiment_analysis.ipynb
 - 활용모델 : BERT-Large, Cased(Original)

|                                | Layers | Embedding Size | Hidden Size | # heads |
| ------------------------------ | -----: | -------------: | ----------: | ------: |
| `BERT-Large, Cased(Original)`  |     24 |           1024 |        1024 |      16 |

- <b>실행 방법</b>  
<t>1. 데이터 출처란 URL 통해 `EmotionLines_friends_annotation.tar` 다운로드 후 압축해제<br>
<t>2. 'friends_dev.json', 'friends_test.json', 'friends_train.json' 총 3개의 파일만 본인의 Google Drive 업로드<br>
<t>3. 모든 셀 실행<br>
<t>4. 초기 Colab ↔ Google Drive간 연동을 위해 Colab 셀 결과 URL 클릭 후 할당받은 인증번호 입력 및 Enter


- <b>데이터 출처</b>  
<t>[EmotionLines Friends](http://doraemon.iis.sinica.edu.tw/emotionlines/download.html)


- <b>참고문헌 및 코드<br>
<t>[1. Google Research Github](https://github.com/google-research/bert)<br>
<t>[2. 네이버 영화리뷰 감성분석 with Hugging Face BERT](https://colab.research.google.com/drive/1tIf0Ugdqg4qT7gcxia3tL7und64Rv1dP)<br>
<t>[3. Emotions classification with ELECTRA](https://github.com/jiwonny/nlp_emotion_classification/blob/master/friends_electra.ipynb)<br>
