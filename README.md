# Quang Minh Khoa Le

**Undergraduate researcher in Surgical AI & Medical Computer Vision**  
Computer Science Engineering &middot; Vietnamese-German University &times; Frankfurt University of Applied Sciences 
(Double Degree, 2023 &ndash; 2027)

Grade 1.2/1.0 (equiv. GPA 3.8/4.0)  

[CV](https://drive.google.com/file/d/1KXJ-4CIbiRFFUKGfoSnFpJNG_xE9CUK0/view?usp=drive_link) &middot; [LinkedIn](https://linkedin.com/in/quangminhkhoale) &middot; [Email](mailto:lequangminhkhoa@gmail.com)

---

### About

Hello, I am an undergraduate researcher working on AI in Medical. Currently, I am researching about Surgical AI; specifically, I am working on AR guided for Laparoscopic Surgery. 

I have no peer-reviewed publications yet. Results below come from my own experiments, competition leaderboards, or unpublished technical reports, and are labelled as such.

---

### Research

* **VGU AI Lab &mdash; Researcher** *(2025 &ndash; Present)*
  * **Liver landmark segmentation on L3D** &mdash; [surgical_ai](https://github.com/KhoaTryToCode/surgical_ai) *(Aug &ndash; Oct 2026)*  
    16 controlled experiments: TopoNet replication, Mask2Former baselines, B&eacute;zier curve heads, junction-based query steering, temporal prototype attention.  
    Found a pose shift between splits (extreme-traction frames: 15.6% of validation vs. 8.0% of training) and moved to pose-stratified, patient-disjoint 5-fold splits.  
    Best model (pose-stratified temporal Mask2Former): 71.9% macro Dice, 15.4 px ASSD on the official test split, vs. 69.6% macro Dice for the best published method (BCRNet, as reported in its paper; not yet re-run under the same protocol). Written up as an unpublished technical report.
  * **l3d-bench: a fair re-evaluation** &mdash; [l3d-bench](https://github.com/KhoaLeQuangMinh/l3d-bench) *(Nov 2026, in progress)*  
    Retraining published methods (TopoNet, BCRNet, A2ONet, D2GPLand) under one split protocol and one metric, so comparisons with my models are like-for-like.
  * **Landmark-free 3D&ndash;2D registration** *(Oct 2026 &ndash; Present, private repo)*  
    Aligning preoperative 3D liver models with laparoscopic frames (P2I-LReg). Current stage: dataset exploration, 3D geometry, preprocessing.

* **AI in Medical Applications Lab (AIMA) &mdash; Researcher** *(2025 &ndash; Present)*
  * **MRI + PET Alzheimer's classification** &mdash; [coding_space](https://github.com/KhoaLeQuangMinh/coding_space) *(May &ndash; Jul 2026)*  
    MRI-only, PET-only and fusion baselines on paired ADNI scans; replication of HOPE (ordinal prototype learning) for MCI progression; experiments with modified (ordinal) triplet losses.
  * **SuStaIn-guided progression prediction** &mdash; [ebm_guide_ordinal](https://github.com/KhoaLeQuangMinh/ebm_guide_ordinal) *(Jul &ndash; Aug 2026)*  
    Multi-head 3D ResNet-18 that predicts SuStaIn subtype and stage from a single T1 MRI; exploratory experiments on separating progression velocity from severity using cross-sectional data.
  * **Segmentation competitions** while at AIMA: 1st place in AIO 2025 Liver Tumor Segmentation and 13th place in the AI Vietnam Warm-up Skin Lesion Segmentation (see [Competitions](#competitions)).

* **Small Multimodal Models for Tropical Disease Diagnosis** &mdash; [repo](https://github.com/KhoaLeQuangMinh/Small-Multimodal-Models-for-Clinical-Diagnosis) *(Sep 2026 &ndash; Present)*  
  Group project supervised by Dr. Tran Duc Khanh (VGU). Prepared the dataset through multi-stage label verification of tropical-disease cases from MultiCaRe, and developed the LightRAG knowledge-graph retrieval benchmarks and, jointly, the four-stage "dual-brain" pipeline (disease-guide knowledge graph, patient-case memory retrieval, hub-suppression ranking, constrained chain-of-thought with Qwen2.5-3B). Team result: 48.2% top-1 / 72.3% top-3 accuracy on a 365-case test set, vs. 7.7% top-1 for the zero-shot base model. Currently working on fine-tuning and multi-agent approaches.

* **AIO Vietnam &mdash; Student / Member** *(2025 &ndash; 2026)*  
  Studied and passed 4 modules: Data Analysis & Data Science, ML/DL, Computer Vision & NLP, GenAI/LLMs. I write about fundamentals in my [AIO Diary](https://wood-note-e64.notion.site/AIO2025-Diary-1f5bfaabd5a180229aacea01946765ef) blog.

---

### Competitions

| Result | Competition | What I did |
|:---|:---|:---|
| **1st place** (Dice 0.972) | AIO 2025 Liver Tumor Segmentation (Kaggle) &mdash; [repo](https://github.com/KhoaLeQuangMinh/3D_Liver_Segmentation) | 2D UNet++ cascade ensemble + 3D largest-connected-component post-processing |
| **13th place** (score 0.876) | AI Vietnam Warm-up: Skin Lesion Segmentation &mdash; [repo](https://github.com/KhoaLeQuangMinh/Skin_Lesion_Segmentation) | Hair-removal preprocessing, CLAHE, hybrid Focal-Tversky / BCE / surface loss |
| Top 72 (Round 1) | Viettel AI Race &mdash; Novel View Synthesis &mdash; [repo](https://github.com/KhoaLeQuangMinh/self-cali-gs-viettel) | Pose refinement (Self-Cali-GS) + 2D Gaussian Splatting pipeline |
| 150th &rarr; 80th &rarr; 50th (Rounds 1&ndash;3), team of 5 | HCMC AI Challenge 2026, video retrieval &mdash; [team repo](https://github.com/AIVIETNAM-AIO-Dewey/AIC-2026) | Built the Vietnamese speech-to-text (PhoWhisper) pipeline and region captioning (DAM) for the offline indexing stage |
| Team member | AABW 2026 Track 2, Tasco Maps POI search &mdash; [team repo](https://github.com/XuanSang2005/Agentic-AI) | Main Researcher and Developer of the Algorithm |

---

### Other projects

* **[Vietnamese Speech-to-Text](https://github.com/KhoaTryToCode/STT)** *(Jul 2026, solo)*: PhoWhisper served with FastAPI, a worker queue and Prometheus metrics.
* **[SmartCart LLM Recommender](https://github.com/KhoaLeQuangMinh/LLM-Recommender)** *(Aug 2026, solo)*: PySpark ALS candidate retrieval, re-ranking, Gemini-generated explanations, Flask API, Docker, GitHub Actions tests.
* **[Proof-of-Stake ledger simulation](https://github.com/KhoaLeQuangMinh/Proof_of_Stake)** *(Jun 2026, Java)*: Algorand-style multi-node consensus simulation; groundwork for a team charity-ledger project (private repo).
* **[Traffic simulator](https://github.com/KiwisCodes/traffic-simulator)** *(Nov &ndash; Dec 2025, Java team project)*: JavaFX + SUMO/TraaS. I built the first multithreaded prototype ([Java_OOP](https://github.com/KhoaLeQuangMinh/Java_OOP)): simulation/map managers, traffic lights.
* **[DRIAMS AMR prediction](https://github.com/KhoaLeQuangMinh/DIRIAMS)** *(Oct 2026)*: extended an open-source 1D-CNN for antibiotic-resistance prediction from MALDI-TOF spectra to support binned data and faster loading.
* **[Stock forecasting](https://github.com/KhoaLeQuangMinh/CONQ047)** *(AIO module project)*: two NLinear models on log-returns.
* **[DVC training pipeline](https://github.com/KhoaLeQuangMinh/AI_implementation)** *(Oct 2025)*: data and model versioning practice.
* **[TrackMeRun](https://github.com/hunggiadao/track-me-run-fitness)** *(2024, first-year team project)*: Flask + Arduino Cloud fitness tracker; I built profile, session and goal features.

---

### Tools

* **Medical imaging & CV:** PyTorch, Mask2Former, UNet++, 3D CNNs (ResNet), NiBabel, FreeSurfer, ANTs, Matplotlib, Gaussian Splatting
* **LLM / retrieval:** LightRAG, Qwen2.5, Gemini API, PySpark MLlib
* **Engineering:** Python, Java (OOP, JavaFX, multithreading), C/C++, R / RStudio, Git, Linux, Docker, DVC, GitHub Actions, Flask, FastAPI, LaTeX, Kaggle
