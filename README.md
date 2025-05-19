# 🔎 YouTube API 기반 동영상 검색 웹 애플리케이션 (Flask + JavaScript)

이 프로젝트는 **YouTube Data API v3**를 활용하여 사용자가 입력한 검색어에 대해 관련 동영상 목록을 불러오고, 이를 웹 페이지에 카드 형태로 표시하는 **검색 기반 웹 애플리케이션**입니다.  
간단한 UI와 RESTful API 구조를 기반으로, **외부 API 연동 및 프론트-백엔드 통신 구조**를 직접 구현할 수 있도록 구성되어 있습니다.

---

## 📷 데모 화면

<img width="700" alt="demo" src="https://github.com/user-attachments/assets/9c771d22-adaf-46ba-a634-577ef012f23a" />

---

## 🚀 실행 방법

### 1. 로컬 환경에서 실행
```bash
# 패키지 설치
pip install flask flask-cors google-api-python-client

# API 키 설정 (app.py 또는 config.py 내 직접 입력)
YOUTUBE_API_KEY = "YOUR_API_KEY"

# 서버 실행
python app.py
```

### 2. 구글 코랩에서 실행
```bash
# Ngrok 토큰 등록
!ngrok authtoken <your_token>

# run_server.py 실행
!python run_server.py

# 출력된 주소(https://xxxx.ngrok.io)로 외부 접속 가능
```

---
## 💡 핵심 기능
### 🔎 검색어 입력 후 YouTube API 호출
### 📡 Flask 백엔드에서 검색 결과 JSON 반환
### 🖼 클라이언트에서 영상 목록(썸네일 + 제목) 시각화
### 🌐 fetch API를 이용한 실시간 요청/응답 처리


---
## 🧩 기술 스택
| 영역     | 사용 기술                                         |
| ------ | --------------------------------------------- |
| 백엔드    | Python, Flask, flask-cors                     |
| API 연동 | YouTube Data API v3, google-api-python-client |
| 프론트엔드  | HTML, JavaScript (fetch API)                  |
| 테스트 환경 | Google Colab + Ngrok                          |


---
## 📁 디렉토리 구조
```bash
.
├── app.py
├── run_server.py
├── sample_data
│   ├── anscombe.json
│   ├── california_housing_test.csv
│   ├── california_housing_train.csv
│   ├── mnist_test.csv
│   ├── mnist_train_small.csv
│   └── README.md
└── www
    ├── index.html
    └── static
        └── js
            └── app.js
```

---
## 🛠 향후 개선 방향
### 🔐 API 키를 환경변수 또는 .env 파일로 보안 강화
### ⏱ 영상 길이, 업로드일 등 메타데이터 추가 표시
### 📄 페이지네이션 처리로 결과 10개 이상 표시
### 🧠 검색어 자동완성 기능 또는 인기 검색어 제시

---
## 🧑‍💻 개발자
### 👤 최기영
### 고급 웹 프로그래밍 과제 프로젝트
