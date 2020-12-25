# sa-competition
KU 빅데이터자연어처리 SA competition

#######################
# 한글 감성분석 모델 #
#######################

# 한글 모델 위치 : ./SA-KO/ko-model.py 또는 ko-model.ipynb (같은 모델)

# 한글 Dataset : Naver Sentiment Movie Corpus

# 학습 데이터 위치
!git clone https://github.com/e9t/nsmc.git - Training data set
!git clone https://github.com/apploberry/sa-competition.git - Competition data set

# Output
 - ko_output.csv 생성

# 실행방법
 - google colab에서 실행
 - 다른 환경에서 실행 시에는 필요한 package install 후 실행 (추가로 필요한 package는 source code 참고)
 
    # KO-BART install
    if PRETRAINED_MODEL == "KO-BART":
        !pip install torch==1.7.1+cu101 torchvision==0.8.1+cu101 torchaudio===0.7.0 -f https://download.pytorch.org/whl/torch_stable.html pytorch_lightning
        !pip install git+https://github.com/SKT-AI/KoBART#egg=kobart

    # 한글 문장분리기 설치
    !pip install kss

    # transformers install
    !pip install transformers

    # learning data file download
    !git clone https://github.com/e9t/nsmc.git
    !git clone https://github.com/apploberry/sa-competition.git


#######################
# 영어 감성분석 모델 #
#######################

# 영어 모델 위치 : ./SA-EN/en-model.py 또는 en-model.ipynb (같은 모델)

# 영어 Dataset : Friends Dataset

# 학습 데이터 위치
!git clone https://github.com/apploberry/sa-competition.git - Training and Competition data set

# Output
 - en_output.csv 생성

# 실행방법
 - google colab에서 실행
 - 다른 환경에서 실행 시에는 필요한 package install 후 실행 (추가로 필요한 package는 source code 참고)

    # transformer install
    !pip install transformers

    # learning data file download
    !git clone https://github.com/apploberry/sa-competition.git

