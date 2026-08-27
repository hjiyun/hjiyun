## 홍지윤 (Jiyun Hong) · 이력 상세

고려대학교 빅데이터사이언스학과 석사과정 (2025.09 ~ 2027.02 졸업예정)
Bayesian Computation · LLM / RAG · Synthetic Data · Time-series Anomaly Detection

통계적 추론과 생성형 AI를 결합해 **불확실성을 정량화하고 설명 가능한 의사결정**을 만드는 데 관심이 있습니다.
JKDAS 제1저자 게재 2편, 연구 설계부터 데이터 전처리 · 모델링 · 평가 · 논문화까지 전 과정을 단독으로 수행해 왔습니다.

---

### Research Interests

- **Bayesian Computation** : Stochastic Gradient MCMC (SGLD · SGHMC · SGNHT · AWSGLD), SAMC, Kalman Filter, Gibbs Sampling
- **LLM & RAG Applications** : Retrieval-Augmented Generation, GraphRAG, 자체 호스팅 LLM 서빙과 경량화, 생성 태스크 평가 체계 설계
- **Synthetic Data Generation** : GAN 기반 불균형 데이터 보완과 품질 검증(분포 · 구조 · 판별 3중)
- **Applied Statistics** : 다변량 시계열(VAR · VECM · 공적분), AHP, Bootstrap, 토픽모델링

---

### Publications

**홍지윤** (제1저자), *한국데이터정보과학회지 (JKDAS)*

1. **RAG와 LLM을 활용한 금융 심사 설명력 향상 방안** · JKDAS 27(2), 2025.04
   - 실고객 **139만 건 · 77개 변수** 기반 EXAONE-Deep-7.8B(AWQ) + FAISS + LangChain RetrievalQA 파이프라인 설계
   - BERTScore **0.61 → 0.86 (+41%)**, BM25 **6.71 → 11.67 (+74%)**, Cosine **0.60 → 0.74**
   - 검색 지표가 구조적으로 RAG에 유리한 자가당착을 명시하고 검색 · 생성 2축으로 평가를 분리

2. **SGMCMC-KF 알고리즘을 이용한 시계열 이상치 탐지** · JKDAS 28(2), 2026.04
   - Kalman Filter의 우도 · 기울기와 SGMCMC를 결합한 온라인 파라미터 갱신 알고리즘 설계
   - Apache Kafka 기반 실시간 스트리밍 파이프라인 구현, 배치 처리 **170.8초 → 31초 (5.5배)**
   - NAB 벤치마크 7종 통제 비교. SGLD-KF가 재현율 **100%**를 유지하며 오탐만 4개 구간 전부에서 6~18% 감소

---

### Featured Projects

| Repository | 설명 | 핵심 기술 |
|---|---|---|
| [`SGMCMC-KF`](https://github.com/hjiyun/SGMCMC-KF) | 스트리밍 시계열 이상치 탐지. 배치 170.8초 → 31초, 재현율 100% 유지 | SGMCMC, Kalman Filter, Kafka |
| [`BSS-Keyphrase-Extraction`](https://github.com/hjiyun/BSS-Keyphrase-Extraction) | 준지도 키프레이즈 추출 샘플러. 다봉 사후분포의 로컬 트랩 조건에서 AWSGLD만 수렴(R̂ 1.15) | AWSGLD, SGLD, PU Learning |
| [`fda-compliance-sql`](https://github.com/hjiyun/fda-compliance-sql) | 식품 수출 표시사항 규제 대응. 2,493건 × 3국 전수 진단으로 "FDA 적합 · CODEX 위반" 95건 사전 식별 | PostgreSQL 18, Docker, Streamlit |
| [`synthetic-data-tbt-detection`](https://github.com/hjiyun/synthetic-data-tbt-detection) | AdsGAN 기반 식품 TBT 위반 탐지. 라벨 1:63 불균형 보완, RF 정확도 **87% → 96%** | AdsGAN(SynthCity), Random Forest |
| [`Woongjin_Book_project`](https://github.com/hjiyun/Woongjin_Book_project) | 꿈꾸는 책방: 음성 복제 · 캐릭터 대화 · 그림 기반 동화 창작 3종 AI 파이프라인 | ElevenLabs, GPT-4o-mini, React |

---

### Selected Research (비공개 · 보고서)

- **행정법령 GraphRAG 챗봇** (2025.09 ~ 2025.12, S-CURT 대학원생 멘토)
  Law-Article-Revision 3계층 그래프 + 벡터 이중 DB 설계. 공통 백엔드 위 어댑터로 RAG 7종을 통제 비교해 Typed-RAG가 RAGAS Overall **0.861**로 최고. 종합 점수 대신 지표를 분해해 Instruct-RAG의 answer relevancy 0.883 / faithfulness 0.125 불균형을 포착
- **SAMC-CBS 초고차원 베이지안 변수선택** (2025.06 ~ 2025.11)
  탐색 커널만 상관 기반 제안분포로 교체해 참 신호 검출 **100%** (미검출률 73% → 0%), 오탐률 **10.7%**로 Elastic Net(73.6%) 대비 6.9배 감소
- **스마트팜 작물 생육 예측 및 최적 작물 추천** (2023.11 ~ 2024.05, (주)제레스팜 인턴)
  작물 추천 정확도 **81%** (LGBM), 직접 설계한 "해당 없음" 클래스가 테스트셋에서 precision · recall 모두 **1.00**. 검정 오류를 데이터 구조로 추적해 센서 18대 중 17대분이 동일 환경 중복 측정임을 규명하고 재배치 · 측정 주기 기준 제시
- **한반도 평화지수 산출 및 LDA 담론 교차 검증** (2025.11)
  4영역 14지표 체계와 AHP 가중치 설계(일관성 비율 0.00001), 부트스트랩 1,000회 신뢰구간으로 불확실성 표기
- **LDA + SGLD 하이브리드 토픽모델링** (2025.04 ~ 2025.07)
  Coherence Score **0.421 → 0.705 (+67.7%)**, 토픽 수는 Perplexity · Coherence · Silhouette 전 구간 비교로 결정

---

### Experience

- **고려대학교 빅데이터사이언스학과 석사과정 연구원** (2025.09 ~ 현재)
  Bayesian Computation · LLM/RAG · 합성데이터 기반 AI 응용 연구. 학부연구생 대상 실험 설계와 연구 전 주기 멘토링
- **NRF 과제 참여연구원** : RS-2024-00352792 (2024.05 ~ 2027.04, 학부연구생 단계부터 연속 참여)
- **초격차 산업기반표준 전문인력양성사업** (2025.09 ~ 현재) : 식품 TBT 대응 1 · 2차년도 참여
- **(주)제레스팜(파미트리) 데이터팀 인턴** (2023.11 ~ 2024.05) : AWS EC2 기반 데이터 구조 설계와 SQL 데이터 마트 운영 단독 수행

---

### Awards & Publication

- **한국자료분석학회 하계학술대회 포스터논문 장려상** (2026.06) : BSS-AWSGLD 준지도 키프레이즈 추출 샘플러
- **저서** 『인공지능으로 코딩 없이 게임 만들기 For 프롬프트 활용』 (마린북스, 2026.07)
- **통계학술제 최우수상** (2023.11) : 택시 수요 분석 기반 서비스 개선
- **빅페스타 장려상** (2023.11) : 응급 대응 분석 기반 소방서 위치 최적화
- **삼성휴먼테크 논문대상 동상** (2020.02) : 수면 뇌파 기반 맞춤 알람 장치

---

### Tech Stack

- **Programming** : Python, R, SQL(PostgreSQL), SAS
- **LLM / RAG** : EXAONE-Deep-7.8B(AWQ), Solar · Solar-pro, Gemma-3-4B(8bit + LoRA), GPT-4o-mini, LangChain, FAISS, Chroma, Neo4j, PEFT, bitsandbytes, RAGAS
- **ML / DL** : PyTorch, TensorFlow, scikit-learn, LightGBM, Hugging Face Transformers
- **Bayesian / Statistical** : SGMCMC(SGLD · SGHMC · SGNHT · AWSGLD), SAMC · CBS, Kalman Filter, VAR/VECM · 공적분 · Granger 인과, AHP, Bootstrap, statsmodels
- **Synthetic Data** : AdsGAN(SynthCity), GAN(pix2pix · AC-GAN · DTN), KS 검정 · Wasserstein 거리 · PSI 기반 품질 검증
- **Data & Infra** : Apache Kafka, Docker, PostgreSQL 18, AWS EC2, Git
- **Visualization** : Streamlit, matplotlib, seaborn, QGIS, Tableau
- **Certifications** : SQLD (2024.12), ADsP (2024.09), SAS Base (2023.08)

---

### Contact

- Email : julie2302@naver.com
- GitHub : [github.com/hjiyun](https://github.com/hjiyun)

---

> *데이터의 불확실성을 외면하지 않고, 그 안에서 신뢰할 수 있는 답을 찾아내는 연구를 지향합니다.*
