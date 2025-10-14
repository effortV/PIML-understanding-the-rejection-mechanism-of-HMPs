# AI4MemSci-unraveling-the-rejection-mechanism-of-HMPs
Hydrophilic micropollutants (HMPs), machine learning (ML),, solute-membrane interaction energies (∆Gs–m), Membrane design

The project performs the following steps:

1. **Feature Correlation Analysis**
   - Compute correlation matrices.
   - Visualize correlations with triangular heatmaps.
   - Identify and remove highly correlated features (|r| > 0.7).

2. **Feature Selection with Protection Rule**
   - Retain critical physicochemical descriptors (ΦS, ∆Gs–m, ΦD).
   - Remove redundant or indirectly correlated variables via a recursive graph search.

3. **Substructure**
   - Parse SMILES strings.
   - Detect substructures via SMARTS patterns from `match.txt`.
   - Combine substructure counts with molecular descriptors.

4. **Machine Learning Model**
   - Use **XGBoost Regressor** for performance prediction.
   - Perform **Grid Search (CV=5)** for hyperparameter tuning.
   - Evaluate model using R², MAE, RMSE.

5. **Model Explainability**
   - Apply **SHAP (SHapley Additive exPlanations)** to interpret feature importance.
   - Generate both summary and bar plots.

6. **Partial Dependence Analysis**
   - Compute **single** and **bivariate** PDPs.
   - Export underlying PDP data to Excel for further analysis or publication.



