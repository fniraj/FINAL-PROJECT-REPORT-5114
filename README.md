# Predictive AI Model of Glioblastoma for Effective Outcomes Compared to Clinical Approaches

## **Overview**
Glioblastoma is a highly aggressive brain tumor with poor prognosis and limited treatment options. This project aims to develop a machine learning-based predictive AI model to improve survival prediction and treatment outcomes for glioblastoma patients, providing an alternative to traditional clinical methods.

## **Features**
- Predict survival probabilities at various time points (0.5-year, 1-year, 1.5-year, and 2-year durations).
- Uses advanced machine learning techniques, including:
  - Random Forest
  - XGBoost
  - Support Vector Machines (SVM)
  - Stacking Classifier
- Incorporates survival analysis methods like SHAP and Kaplan-Meier curves for enhanced insights.
- Built to assist healthcare providers in making timely and accurate decisions.

## **Dataset**
- Includes patient demographics, medical history, and treatment details.
- Population Focus: Provides a diverse set of survival data across 0.5, 1, 1.5, and 2-year durations.

## **Methodology**
### **Preprocessing**
1. One-hot encoding applied to categorical variables.
2. Scaling numeric features using StandardScaler.
3. SMOTENC used for balancing minority classes.

### **Feature Selection**
- Top 15 features selected based on ANOVA F-values.

### **Modeling**
1. **Base Models:**
   - Random Forest: Achieves best AUC (0.949 for 0.5-year survival).
   - XGBoost: Known for robust gradient boosting performance.
   - SVM: Captures non-linear interactions with polynomial kernels.
2. **Ensemble Learning:**
   - Stacking Classifier combines predictions from base models to enhance accuracy.

### **Evaluation**
- Metrics include ROC curves, AUC values, and SHAP analysis.
- Kaplan-Meier analysis used for survival probability visualization.

## **Key Findings**
- Random Forest showed the highest predictive power with an AUC of 0.949 for short-term survival.
- SHAP analysis identified key predictors: Age, WHO Grade, Extent of Resection, and Postoperative Neurological Deficits.
- Ensemble methods like Stacking Classifier balanced individual model weaknesses and leveraged complementary strengths.

## **Future Directions**
- Improve ensemble methods for better accuracy in long-term survival predictions.
- Expand datasets to include diverse populations and longitudinal data.
- Explore advanced models like deep learning and genetic/molecular data integration.
- Validate predictions through clinical trials for real-world effectiveness.

## **Support for Clinical Systems**
- **Enhanced Predictive Accuracy:** Provides precise survival predictions to aid early interventions.
- **Feature Insights:** Highlights essential factors for treatment planning.
- **Resource Optimization:** Enables efficient allocation of medical resources.

## **Acknowledgments**
- Tools: Python libraries (Sklearn, XGBoost, SHAP, etc.).
- Credits: Thanks to Dr. Guy Hembroff for guidance throughout the research process.

## **References**
- Wen, P. Y., & Kesari, S. (2008). Malignant gliomas in adults. NEJM.
- Bi, W. L., et al. (2019). AI in cancer imaging: Clinical challenges. CA: A Cancer Journal for Clinicians.
- Breiman, L. (2001). Random forests. Machine Learning.

## **Project Demo**
Explore the working code on [Google Colab](https://colab.research.google.com/drive/1RzLPiBNQovKw1JsvQPJ4XNTb95vdAOKe#scrollTo=xwux0X3enWsB).
