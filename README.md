# Research on Interpretability of Clinical Medicine Based on Machine Learning Predictive Model (基于机器学习预测模型的临床医学可解释性研究)

# Tutorial

```
pip install requirements.txt
```

**Please see the "Tutorial (WorkFlow).ipynb".**

# Reference

The experimental results of the following papers can be implemented using ClinicalTools.

[1] Tseng, P. Y., Chen, Y. T., Wang, C. H., Chiu, K. M., Peng, Y. S., Hsu, S. P., ... & Lee, O. K. S. (2020). Prediction of the development of acute kidney injury following cardiac surgery by machine learning. Critical Care, 24(1), 1-13.

[2] Chen, C., Yang, D., Gao, S., Zhang, Y., Chen, L., Wang, B., ... & Zhou, S. (2021). Development and performance assessment of novel machine learning models to predict pneumonia after liver transplantation. Respiratory research, 22(1), 1-12.

[3] Penny-Dimri, J. C., Bergmeir, C., Reid, C. M., Williams-Spence, J., Cochrane, A. D., & Smith, J. A. (2020, September). Machine learning algorithms for predicting and risk profiling of cardiac surgery-associated acute kidney injury. In Seminars in Thoracic and Cardiovascular Surgery. WB Saunders.

[4] Gong, K., Lee, H. K., Yu, K., Xie, X., & Li, J. (2021). A prediction and interpretation framework of acute kidney injury in critical care. Journal of Biomedical Informatics, 113, 103653.

# ClinicalTools Moudles
- preprocessing
  - description.py
  - imputation.py
  - standardzation.py
- models 
  - FeatureSelection: LASSO OR RFE
  - GridSearchCV (LR, SVC, GNB, GBM, ADA, MLP)
- metrics
  - evaluate.py
  - plot.py
- SHAP
  - SHAP.py
  - selenium_png.py
  - chromedriver: need to download by yourself: https://chromedriver.chromium.org/, and must match the Chrome Version.
- utils
  - colors.py
  - load.py (load large cvs file)

# Results Display

## ROC
![roc](./Example_pics/roc.png)

## Confusion matrix

![confusion_matrix](./Example_pics/Confusion_matrix.png)

## SHAP 

### summary plot
![summary_dot](./Example_pics/summary_dot.png)
![summary_bar](./Example_pics/summary_bar.png)


### dependence plot

![age](./Example_pics/Age.png)
![admission](./Example_pics/Admission.png)

### force plot

![force_plot_0](./Example_pics/force_plot_patients_0.png)
![force_plot_2](./Example_pics/force_plot_patients_2.png)

### decision plot

![decision_plot_65](./Example_pics/patient_65.png)
