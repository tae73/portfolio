# Portfolio

## About Me

ML, Causal Inference, LLM 등의 방법론을 활용하여
개인화, 실험, 추천 등의 태스크에서 현실 문제를 해결합니다.
관측 데이터에서의 인과 효과 추정과 이를 통한 의사결정 최적화에 집중하고 있습니다.

- **Methods**: ML, Causal Inference, LLM
- **Tasks**: Personalization, Experimentation, Recommendation
- **GitHub**: [tae73](https://github.com/tae73)

---

## Projects

### 1. Customer Segmentation & Causal Targeting

> NMF + K-Means 기반 고객 세분화 → HTE 기반 최적 타겟팅 (ROI +200pp)

`Python` `Causal Inference` `NMF` `K-Means` `HTE` `Policy Learning` `Optuna`

Dunnhumby 리테일 데이터(2,500 가구, 260만 거래)를 활용한 2-Track 프레임워크.
Track 1에서 NMF 잠재 요인 모델링과 K-Means 클러스터링으로 7개 고객 세그먼트를 정의하고,
Track 2에서 이질적 처리 효과(HTE) 추정과 정책 학습을 통해 최적 31% 타겟팅 규칙을 도출하여
$7,083 매출 개선(ROI +200pp)을 달성.

**Docs:**
[Track 1 Report (세분화)](https://github.com/tae73/kr_segmentation_causal_targeting_dunnhumby/blob/main/docs/track1_report.md) |
[Track 2 Report (인과추론 & 최적 정책)](https://github.com/tae73/kr_segmentation_causal_targeting_dunnhumby/blob/main/docs/track2_report.md) |
[Segment Profiles](https://github.com/tae73/kr_segmentation_causal_targeting_dunnhumby/blob/main/docs/interview.md)

**Repo:** [kr_segmentation_causal_targeting_dunnhumby](https://github.com/tae73/kr_segmentation_causal_targeting_dunnhumby)

---

### 2. LLM-Factor RecSys (H&M)

> 3-Layer Attribute Taxonomy + KAR Hybrid-Expert Adapter로 Triple-Sparsity 문제 해결

`Python` `LLM` `KAR` `DeepFM` `PyTorch` `Recommendation Systems` `Hydra`

H&M 패션 추천에서 Triple-Sparsity 문제(32.1% sparse users, 99.98% sparse matrix)를 해결하기 위해
LLM으로 추출한 다층 속성(L1+L2+L3)의 점진적 가치를 검증.
DeepFM + KAR 아키텍처 기반 discovery-oriented 추천 시스템.

**Docs:**
[Research Design](https://github.com/tae73/llm-factor-recsys-hnm/blob/main/docs/research_design/hm_unified_project_design.md) |
[Evaluation Methodology](https://github.com/tae73/llm-factor-recsys-hnm/blob/main/docs/evaluation_methodology.md) |
[Prompt Design](https://github.com/tae73/llm-factor-recsys-hnm/blob/main/docs/prompt_design.md) |
[Cold Start Analysis](https://github.com/tae73/llm-factor-recsys-hnm/blob/main/docs/cold_start_analysis.md) |
[MLOps Design](https://github.com/tae73/llm-factor-recsys-hnm/blob/main/docs/mlops_design/hm_mlops_design.md)

**Repo:** [llm-factor-recsys-hnm](https://github.com/tae73/llm-factor-recsys-hnm)

---

### 3. RTB Debiasing & Bid Optimization

> Win Selection Bias Debiasing (ESMM-WC, DR) + First-price Bid Optimization (<100ms serving)

`Python` `RTB` `Causal Inference` `ESMM` `Doubly Robust` `LightGBM` `MLflow`

Real-Time Bidding에서 Bid→Win→Click 퍼널의 Win Selection Bias를 ESMM-WC 및 ESCM²-WC(DR)
이중 강건 추정으로 교정. Win Tower 이중 목적 설계(CTR 디바이싱 성향 점수 + 입찰 셰이딩, AUC ~0.91)와
프로덕션 서빙(<100ms latency) 포함.

**Docs:**
[Data Preparation](https://github.com/tae73/rtb_ipinyou/blob/main/docs/research_design/00-data-preparation.md) |
[Prediction Models](https://github.com/tae73/rtb_ipinyou/blob/main/docs/research_design/01-prediction-models.md) |
[Win Rate Analysis](https://github.com/tae73/rtb_ipinyou/blob/main/docs/research_design/02-win-rate-analysis.md) |
[Bid Optimization](https://github.com/tae73/rtb_ipinyou/blob/main/docs/research_design/03-bid-optimization.md) |
[Causal Analysis](https://github.com/tae73/rtb_ipinyou/blob/main/docs/research_design/04-causal-analysis.md) |
[Serving](https://github.com/tae73/rtb_ipinyou/blob/main/docs/research_design/05-serving.md)

**Repo:** [rtb_ipinyou](https://github.com/tae73/rtb_ipinyou)
