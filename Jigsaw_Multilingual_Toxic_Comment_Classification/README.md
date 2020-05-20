# Jigsaw Multilingual Toxic Comment Classification

- [대회 링크](https://www.kaggle.com/c/jigsaw-multilingual-toxic-comment-classification/overview)



## 대회 설명

본 대회는 Jigsaw라는 회사에서 주관한 대회입니다. [Jigsaw](https://jigsaw.google.com/)는 전 세계가 직면한 안전 과제를 해결하기 위한 기술을 개발하는 Alphabet의 자회사로, 온라인 검열의 중단, 디지털 공격의 위협 완화, 폭력적인 극단주의 저지, 온라인 권리침해로부터 사용자 보호 등의 다양한 과제를 놓고 연구하고 있는 회사입니다.

본 대회는 어떤 comment가 주어졌을 때 그 comment가 악성 댓글인지 아닌지를 분류하는 대회입니다. comment는 영어뿐만 아니라 여러 국가의 언어로 구성되어 있습니다. 여러 국가의 언어로 구성되어 있는 comment가 악성 댓글이면 1, 악성 댓글이 아니면 0으로 구분하는 것이 최종 목적입니다.

## 참여 일지

- 2020.04.27

  - 대회 내용 파악
  - [`jigsaw_multilingual_preprocessing.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Jigsaw_Multilingual_Toxic_Comment_Classification/jigsaw_multilingual_preprocessing.ipynb): [공개 커널 분석] BERT 적용을 위해 `comment text`를 `input_ids`, `input_mask`, `segment_ids`로 전처리한 베이스라인
- 2020.04.28 ~ 04.29
  - [`jigsaw_multilingual_getting_started.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Jigsaw_Multilingual_Toxic_Comment_Classification/Jigsaw_multilingual_getting_started.ipynb): [공개 커널 분석] 베이스라인 submission
  - TF2 코드여서 뒷부분은 약간 이해가 되지 않았음
- 2020.04.29 ~ 04.30
  - [`zero_to_transformers&BERT.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Jigsaw_Multilingual_Toxic_Comment_Classification/zero_to_transformers%26BERT.ipynb): [공개 커널 분석] simple RNN, Word Embeddings, LSTM, GRU, Bi-Directional RNN, seq2seq, Attention Models, Transformers, BERT 개념 및 기본 코드 활용 방법 스터디용 커널 (NLP 입문자에게 강추!)
- 2020.04.30
  - `jigsaw_EDA.ipynb`: [공개 커널 분석] jigsaw comment 데이터 EDA (각종 인사이트 도출)
- 2020.05.01
  - [`xlm-roberta-large.ipynb`]([https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Jigsaw_Multilingual_Toxic_Comment_Classification/TPU_%20XLM-Roberta.ipynb](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Jigsaw_Multilingual_Toxic_Comment_Classification/TPU_ XLM-Roberta.ipynb)): [공개 커널 분석] xlm-roberta-large를 활용한 모델링 [LB 0.9375]
  - 코드는 짧지만 성능이 좋은 커널 (현재 최대 vote 공유 커널)
  - 캐글 TPU 기준으로 돌리는데 1시간 소요, 커밋하는데도 꽤 많은 시간 소요
- 2020.05.09
  - [`class_balance_with_pytorch/XLA.ipynb`](https://github.com/BaekKyunShin/Kaggle-Competition-Including-Dacon/blob/master/Jigsaw_Multilingual_Toxic_Comment_Classification/class_balance_with_pytorch_XLA.ipynb): [공개 커널 분석] 훈련 데이터의 label은 10배 이상 심하게 불균형함. 따라서 upsampling 혹은 downsampling으로 데이터 간 밸런스를 맞출 필요가 있음. 파이토치 코드이긴 하지만 데이터 밸런싱을 하는 방법에 대해 익힐 수 있는 커널
  - `xlm-roberta-large.ipynb`과 공개 커널 중 성능이 더 높은 roberta와 앙상블하여 제출했지만 공개 커널의 성능보다 더 좋지 않았음
- 2020.05.14
  - `Jigsaw TPU: BERT with Huggingface and Keras.ipynb`: [공개 커널 분석] `xlm-roberta-large.ipynb`와 동일하되 모델을 BERT로 수정한 코드 분석
- 2020.05.17 ~ 05.21
  - pytorch tutorial 학습: [What is PyTorch?](https://pytorch.org/tutorials/beginner/blitz/tensor_tutorial.html#sphx-glr-beginner-blitz-tensor-tutorial-py), [Autograd](https://pytorch.org/tutorials/beginner/blitz/autograd_tutorial.html#sphx-glr-beginner-blitz-autograd-tutorial-py), [Neural Networks](https://pytorch.org/tutorials/beginner/blitz/neural_networks_tutorial.html), [Training a Classifier](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html), [Learning pytorch with examples](https://pytorch.org/tutorials/beginner/pytorch_with_examples.html) [pytorch nn tutorial](https://pytorch.org/tutorials/beginner/nn_tutorial.html)
  - `Pytorch-XLA: Understanding TPU's and XLA.ipynb`: [공개 커널 분석] TPU 및 Pytorch-XLA 소개 및 활용방안

