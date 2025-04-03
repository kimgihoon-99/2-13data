한국복지패널 데이터 시각화 및 통계 분석
이 프로젝트는 한국복지패널 데이터를 기반으로 다양한 시각화와 기초 통계 분석(T검정) 을 수행하여, 데이터를 직관적으로 이해하고 통계적으로 해석할 수 있도록 구성되었습니다.

📌 주요 기능
mpg.csv, economics.csv 등 실험 데이터셋을 활용한 시각화

plotly, matplotlib 기반의 HTML 시각화 결과 제공

T-test를 통한 집단 간 평균 비교 분석

웹 브라우저로 시각화 파일을 바로 열 수 있도록 자동 실행

📁 디렉토리 구조
bash
복사
편집
2-13data-master/
├── .gitignore
├── README.md               # (이 파일)
├── bar_plot.html           # 자동차 종류별 막대 그래프
├── box_plot.html           # 연비 관련 박스플롯
├── line_plot.html          # 시간에 따른 소비율 변화
├── scatter_plot.html       # 도시연비 vs 고속도로연비 산점도
├── size_plot.html          # 크기에 따른 시각화 (추정됨)
├── interactive.py          # plotly 기반 시각화 자동 생성
├── t_test.py               # T-test 기반 평균 비교 분석
└── data/
    ├── mpg.csv             # 자동차 연비 데이터
    └── economics.csv       # 경제 데이터
⚙️ 설치 및 실행 방법
1. 패키지 설치
bash
복사
편집
pip install pandas plotly scipy matplotlib
2. 시각화 실행
bash
복사
편집
python interactive.py
실행하면 .html 파일로 저장되며, 웹 브라우저가 자동으로 열립니다.

3. 통계 분석 실행
bash
복사
편집
python t_test.py
Compact와 SUV 차량의 연비 차이에 대한 독립표본 T검정 수행 결과를 확인할 수 있습니다.

🧪 사용된 분석 기법
✅ 시각화
plotly.express.scatter – 산점도

plotly.express.bar – 막대그래프

plotly.express.line – 시계열 선그래프

plotly.express.box – 박스플롯

✅ 통계 분석
T-test (독립표본)

두 집단의 평균 차이가 통계적으로 유의미한지 분석

예시: Compact vs SUV 차량의 도시 연비 비교

📚 참고
Python 3.7+

한국복지패널 기반 예제 데이터셋 (mpg.csv, economics.csv)

프로젝트 기반 학습 목적 (시각화 + 추론통계)
