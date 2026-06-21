# Fetal_Health_RandomForest
本專案目標是透過隨機森林演算法與 SMOTE 技術，建立一個高敏感度的胎兒健康風險預測模型，並結合統計學檢定與 SHAP 可解釋性分析，揭示影響胎兒病理診斷的核心關鍵生理指標。
### 資料來源 (Dataset Citation)
- **Kaggle 資料集維護者**：[Larxel (andrewmvd)](https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification)
- **原始學術文獻引用 (Original Research)**：
  Ayres de Campos et al. (2000) *SisPorto 2.0 A Program for Automated Analysis of Cardiotocograms.* J Matern Fetal Med 5:311-318.

---

### 🗂️分析工具
- 統計分析工具：Kruskal-Wallis Test, Dunn's Post-hoc Test (搭配 Bonferroni 校正) — 用於特徵顯著性檢定
- 資料平衡工具：SMOTE (Synthetic Minority Over-sampling Technique) — 用於解決類別不平衡問題。
- 機器學習工具：Random Forest Classifier — 用於核心分類預測模型。
- 模型解釋工具：SHAP (SHapley Additive exPlanations) — 用於黑盒子模型決策之視覺化解構。

---

### 📊使用資料集:
- 資料來源：Fetal Health Classification(https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification)
- 資料內容: 使用 *prolongued_decelerations, abnormal_short_term_variability, percentage_of_time_with_abnormal_long_term_variability, accelerations, uterine_contractions,baseline_value*
- 目標函數：將目標變數分為三類:Normal, Suspect, Pathological
