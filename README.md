#partyroom_review_analysis

##🏠프로젝트 제목<br>
경기도 성남시 모란역 인근 파티룸 A,B,C 리뷰 분석

---

##🎯프로젝트 목표<br> 
고객 이용 행태 및 만족 요인을 정량적으로 파악하여<br>
신규 파티룸 창업 시 **입지/서비스/운영 전략 수립**을 위한 기초자료로 활용하는 것을 목표로 함

---

##📊분석 항목
- 파티룸 수요 분석
- 충성도 분석
- 키워드 분석
- 이벤트 유형 분석
- 긍*부정 요인 분석

---

##🧰사용 기술 및 라이브러리<br>
**언어**
- Python
- Word(기획안 리포트, 시각 자료 정리용)

**라이브러리**
- pandas: 데이터 불러오기, 데이터프레임 형태로 저장
- ast: 문자열 형태의 리스트를 실제 python 객체로 변환
- konlpy: 한국어 형태소 분석(Okt 분석기 활용)
- collections: 단어 출현 빈도 계산 및 키워드 집계에 활용(Counter)
- re: 정규표현식을 이용해 리뷰 텍스트 분리, 불필요한 공백 제거

---

##📂폴더 구조
```
PARTYROOM_REVIEW_ANALYSIS/
├── data/ # 원본 및 전처리된 리뷰 데이터
│ ├── partyroom_A_review.xlsx
│ ├── partyroom_B_review.xlsx
│ ├── partyroom_C_review.xlsx
│ ├── A_preprocessing.xlsx
│ ├── B_preprocessing.xlsx
│ └── C_preprocessing.xlsx
│
├── notebooks/ # 크롤링, 전처리, 분석 코드
│ ├── 01_crawling.ipynb
│ ├── 02_preprocessing.ipynb
│ └── 03_analysis.ipynb
│
├── results/ # 분석 결과 시각화 이미지
│ ├── 01_A파티룸_수요_분석.JPG
│ ├── 02_A파티룸_충성도지표.JPG
│ ├── 03_A파티룸_키워드분석.JPG
│ ├── 04_A파티룸_이벤트분류.JPG
│ ├── 05_A파티룸_긍정_부정분석(시설).JPG
│ ├── 06_A_B_C파티룸_키워드_순위비교.JPG
│ └── 07_A_B_C파티룸_이벤트성_방문비율.JPG
│
└── README.md
```  

---

##💡주요 인사이트
- **12월, 주말, 올나잇 시간대**에 수요 집중
- **이벤트성 모임**이 파티룸 방문의 주요 동기로 작용
- **시설 만족도**는 만족도가 높지만, **재방문율은 낮은 편** -> 고객 유지 전략 필요
- **B,C파티룸**은 리뷰 수 부족으로 인식 파악 한계 -> **리뷰 작성 유도 방안** 필요
- **화장실/주차 불만**등 불편 요소는 향후 신규 창업 시 **접근성과 편의성 강화 방향**시사

---

##🚀실행 방법
1. '01_crawling.ipynb' 실행(네이버 지도 리뷰 데이터 수집)
2. '02_preprocessing.ipynb' 실행(데이터 전처리)
3. '03_analysis.ipynb'(데이터 정량적 분석)

> 🔎참고:<br>
> - '01_crawling'은 네이버 지도 구조 변경 시 CSS 선택자 업데이트 필요
> - '03_analysis'의 재방문률 계산은 B/C 데이터 구조에 따라 별도 처리 필요

---

##👩‍💻작성자
**최다연(Dayeon Choi)**
- dayoun0616@gmail.com
- 데이터 기반 인사이트 도출과 소비자 만족도 분석에 관심이 있습니다.
