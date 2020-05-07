# Tweet Sentiment Extraction

- [대회 링크](https://www.kaggle.com/c/tweet-sentiment-extraction/overview)



## 대회 설명



## 참여 일지

- 2020.04.20 ~ 04.26
  - 대회 내용 파악
  - [`basic_preprocessing_and_EDA.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/basic_preprocessing_and_EDA.ipynb), [`EDA_and_modeling.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/EDA_and_modeling.ipynb), [`sentiment_extraction_understanding_metric_and_EDA.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/sentiment_extraction_understanding_metric_and_EDA.ipynb), [`BERT_base_uncased_pytorch.ipynb`]([https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/BERT_base_uncased%20pytorch.ipynb](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/BERT_base_uncased pytorch.ipynb)): [공유 커널 분석] 전처리, EDA, pytorch를 활용한 BERT 모델링 
- 2020.05.03
  - [`tensorflow_roBERTa_training.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/tensorflow_roBERTa_training.ipynb), [`tensorflow_roBERTa_inference`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/tensorflow_roBERTa_inference.ipynb): [공유 커널 분석] roBERTa 활용 모델 훈련 및 inference model활용 예측 [LB 0.706]
  - 모델 훈련과 예측을 하나의 노트북에서 하기에는 시간이 오래 걸려 모델 훈련과 inference 노트북을 나누었음. 모델 훈련은 대략 1시간 소요, 모델 훈련 후 weight를 h5파일로 저장하여 inference 노트북에서 저장한 weight를 그대로 활용하여 예측 (예측 소요시간은 10분 이내)
  - encoding되는 데이터에 대해 직관적으로 그림을 그려 보여주어 도움이 많이 된 커널임
- 2020.05.04 ~ 05.05
  - [`tensorflow_roBERTa_inference_postprocess_LB_0.713.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Tweet_Sentiment_Extraction/tensorflow_roBERTa_inference_postprocess_LB_0.713.ipynb): [공유 커널 분석] 기존의 tensorflow_roBERTa_inference 커널에서 1) convolutional layer 추가, 2) Learning rate 추가, 3) `model.fit()`에서 epochs와 batch_size 수정, 4) post-processing 한 커널을 활용하여 모델 훈련 및 inference model 활용 예측 [LB 0.713]
  - 모델 훈련에 대략 3시간 소요
- 2020.05.07
  - `tensorflow_roBERTa_inference_postprocess_LB_0.713`와 `tensorflow_roBERTa_inference`를 앙상블해보니 LB 0.710으로 성능 향상이 없었음
