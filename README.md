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
<t>[https://github.com/e9t/nsmc.git](https://github.com/e9t/nsmc.git)

- <b>참고문헌 및 코드</b>    
 <t>[1. 네이버 영화리뷰 감성분석 with Hugging Face BERT](https://colab.research.google.com/drive/1tIf0Ugdqg4qT7gcxia3tL7und64Rv1dP#scrollTo=P58qy4--s5_x)<br>
 <t>[2. BERT로 네이버 영화 리뷰데이터 분류하기](http://yonghee.io/bert_binary_classification_naver/)<br>
 <t>[3. monologg/KoELECTRA Gitgub](https://github.com/monologg/KoELECTRA)<br>
 <t>[4. BERT에 대해 쉽게 알아보기](https://ebbnflow.tistory.com/151)<br>
<br>


### 2. Friends 영화 대본 데이터 감정 분석

 - 코드 :  BERT_friends_sentiment_analysis.ipynb
 - 활용모델 : BERT-Large, Cased (Original)
 24-layer, 1024-hidden, 16-heads, 340M parameters

- <b>실행 방법</b>  
<t>1.  `friends_train.json`, `friends_dev.json`, `friends_test.json`을 압축한 파일 `Friends.zip`을 업로드한 후 unzip 실행  
<t>2.  이후 모든 셀 실행을 통해 <b>1) 데이터 전처리, 2) 모델 구현 및 학습, 3) test set 결과 확인 및 csv 파일 변환</b> 가능.


- <b>데이터 출처</b>  
<t>[http://doraemon.iis.sinica.edu.tw/emotionlines/index.html](http://doraemon.iis.sinica.edu.tw/emotionlines/index.html)


- <b>참고문헌 및 코드</b>  
<t>[모델 학습 관련 소스코드 : https://colab.research.google.com/drive/1tIf0Ugdqg4qT7gcxia3tL7und64Rv1dP](https://colab.research.google.com/drive/1tIf0Ugdqg4qT7gcxia3tL7und64Rv1dP)


<br>
