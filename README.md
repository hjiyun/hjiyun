## 홍지윤 (Jiyun Hong)

고려대학교 빅데이터사이언스학과 석사과정 (2025.09 –) · 지도교수 전수영
Bayesian Computation · LLM/RAG · Synthetic Data · Multimodal AI

통계적 추론과 생성형 AI를 결합해 **불확실성을 정량화하고 설명 가능한 의사결정**을 만드는 데 관심이 있습니다.

---

### Research Interests

- **Bayesian Computation** — Stochastic Gradient MCMC (SGLD, SGHMC, SGNHT), Kalman Filter, Gibbs Sampling
- **LLM & RAG Applications** — Retrieval-Augmented Generation, Domain-Specific QA, Explainability
- **Synthetic Data Generation** — GAN 기반 불균형 데이터 보완, 산업 안전·식품 분야 응용
- **Multimodal AI** — 텍스트·정형·시계열 데이터를 통합한 의사결정 모델

---

### Publications

**홍지윤** (제1저자), *한국데이터정보과학회지 (JKDAS)*

1. **RAG와 LLM을 활용한 금융 심사 설명력 향상 방안** — JKDAS 27(2), 2025.04
   - EXAONE-Deep-7.8B + FAISS + LangChain RetrievalQA 파이프라인 설계
   - 신한금융 실고객 데이터 **139만 건** 분석
   - BM25 **6.71 → 11.67**, BERTScore **0.61 → 0.86** 개선

2. **SGMCMC-KF 알고리즘을 이용한 시계열 이상치 탐지** — JKDAS
   - Kalman Filter + SGMCMC (SGLD · SGHMC · SGNHT) 결합 모델 제안
   - Apache Kafka 기반 실시간 스트리밍 파이프라인 구현
   - **NAB 벤치마크 F1·정확도 최우수** 성능 확보

---

### Featured Projects

| Repository | 설명 | 핵심 기술 |
|---|---|---|
| [`rag`](https://github.com/hjiyun/rag) | RAG 기반 금융 심사 설명 시스템 | EXAONE, FAISS, LangChain |
| [`SGMCMC-KF`](https://github.com/hjiyun/SGMCMC-KF) | 스트리밍 시계열 이상치 탐지 | SGMCMC, Kalman Filter, Kafka |
| [`synthetic-data-tbt-detection`](https://github.com/hjiyun/synthetic-data-tbt-detection) | AdsGAN 기반 식품 TBT 탐지 — RF **87% → 96%**, F1 **+33%p** | AdsGAN, Random Forest |
| [`fda-compliance-sql`](https://github.com/hjiyun/fda-compliance-sql) | FDA 식품 라벨링 규제 준수 SQL 시스템 | SQL, 데이터 모델링 |

---

### Experience

- **NRF 과제 참여연구원** — RS-2024-00352792 (2024.05 – 2027.04)
- **초격차 산업기반표준 사업** — 식품 TBT 대응 1·2차년도 참여
- **제레스팜 데이터팀 인턴** — 스마트팜 작물 생육·수확 예측 모델 (R² **0.99**)

---

### Awards

- **삼성휴먼테크 논문대상 동상** (2020)
- **통계학술제 최우수상** (2023)
- **빅페스타(BigFesta) 장려상** (2023)

---

### Tech Stack

- **Programming** — Python, R, SQL, SAS
- **ML / DL / LLM** — PyTorch, TensorFlow, scikit-learn, Hugging Face, LangChain, FAISS
- **Bayesian / Statistical** — SGMCMC, Gibbs Sampling, Kalman Filter, LDA
- **Data & Infra** — Apache Kafka, AWS, Tableau, QGIS, Neo4j, Git
- **Certifications** — SAS Base, ADsP, SQLD

---

### Contact

- Email — julie2302@korea.ac.kr
- GitHub — [github.com/hjiyun](https://github.com/hjiyun)

---

> *데이터의 불확실성을 외면하지 않고, 그 안에서 신뢰할 수 있는 답을 찾아내는 연구를 지향합니다.*
