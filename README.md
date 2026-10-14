
# Machine Learning – ML_PCOM7E e-Portfolio

**Student Name:** Essa Albuainain  
**Module:** Machine Learning (ML_PCOM7E)  
**Institution:** University of Essex Online  
**Assessment:** Individual e-Portfolio  
**Portfolio URL:** https://essaalbuainain.github.io/machine-learning-eportfolio/

---

## Introduction and Learning Outcomes

This e-Portfolio presents evidence of my learning across Units 1–12, including practical activities, collaborative discussions, group and individual projects, tutor feedback, and critical reflection.

The evidence addresses four learning outcomes: understanding legal, social, ethical and professional issues; assessing dataset suitability; applying and evaluating machine-learning methods; and collaborating effectively in virtual teams.

My development progressed from data exploration and regression to clustering, neural networks, optimisation, explainability and responsible AI.

---

# 1. Foundations – Units 1–3

## Unit 1 – Introduction to Machine Learning

Unit 1 introduced supervised and unsupervised learning, the machine-learning lifecycle, and the relationship between data quality and model performance. I recognised that selecting an algorithm requires understanding the problem, available evidence and practical limitations.

## Unit 2 – Exploratory Data Analysis

The Auto-MPG activity investigated distributions, missing values and correlations. Six horsepower values were missing, while vehicle weight, displacement and cylinders showed negative relationships with MPG.

The exercise demonstrated why data auditing should precede modelling and why correlation must not be confused with causation.

![Auto-MPG Correlation Heatmap](assets/Auto-MPG%20Correlation%20Heatmap.jpeg)

*Figure 1. Auto-MPG correlation analysis.*

## Unit 3 – Correlation and Regression

I explored covariance, Pearson correlation, linear regression and polynomial regression. Comparing these approaches demonstrated how model assumptions and complexity affect fitted relationships and the risk of overfitting.

![Correlation and Regression Results](assets/Correlation%20and%20Regression%20Results.jpg)

*Figure 2. Correlation and regression results.*

---

# 2. Applied Regression – Unit 4

The practical work examined fuel-consumption relationships and population–GDP indicators from 2001 to 2021. The fitted regression illustrated the limitations of explaining complex outcomes using a single predictor.

I learned that an observed association does not automatically establish predictive reliability or causal influence.

![Population GDP Regression](assets/Population%E2%80%93GDP%20Regression.png)

*Figure 3. Population–GDP regression.*

---

# 3. Similarity and Clustering – Units 5–6

## Unit 5 – Jaccard Distance

The Jaccard exercise compared categorical observations:

| Comparison | Distance |
|---|---:|
| Jack–Mary | 0.7273 |
| Jack–Jim | 0.4444 |
| Jim–Mary | 0.9231 |

Jack and Jim were the most similar pair. The activity showed how attribute representation affects similarity calculations.

![Jaccard Calculations](assets/Jaccard%20Calculations.png)

*Figure 4. Jaccard calculations.*

## Unit 5 – K-Means Wiki

The wiki activity examined cluster assignment, centroid updates and sensitivity to initialisation. I learned that algorithmically generated clusters require interpretation and validation; silhouette analysis is one possible approach (Rousseeuw, 1987).

![K-Means Wiki](assets/Wiki%20.jpeg)

*Figure 5. K-Means wiki evidence.*

## Unit 6 – Iris Clustering

I applied K-Means with three clusters to the Iris dataset. This demonstrated the difference between unsupervised groupings and known classification labels.

![Iris Clustering](assets/Iris%20Clustering.png)

*Figure 6. Iris clustering results.*

---

# 4. Unit 6 Group Project – Airbnb NYC

## Project and Results

The group investigated Airbnb NYC listing-price prediction and supply segmentation using the Airbnb Open Data dataset (Dgomonov, 2019).

The regression models included Linear Regression, Random Forest (Breiman, 2001) and XGBoost (Chen and Guestrin, 2016).

| Model | R² |
|---|---:|
| Linear Regression | 0.501 |
| Tuned Random Forest | 0.608 |
| Untuned XGBoost | 0.617 |
| Tuned XGBoost | **0.623** |

Although tuned XGBoost performed best, errors for expensive listings limited the reliability of some pricing recommendations.

![Airbnb Model Comparison](assets/Airbnb%20Model%20Comparison%20and%20Segmentation2.png)

*Figure 7. Regression performance.*

K-Means identified four supply-side segments: high-turnover performers, listed-but-not-booking properties, commercial operators and dormant hosts.

![Airbnb Supply Segmentation](assets/Airbnb%20Model%20Comparison%20and%20Segmentation1.png)

*Figure 8. Airbnb supply segmentation.*

## Individual Contribution and Teamwork

I completed my assigned part of the group project and reviewed the full research report to check its overall quality, consistency and presentation before submission.

Reviewing the complete report helped me understand how individual contributions fit together and why a group submission requires a coherent argument rather than separate pieces of analysis.

My peer self-evaluation score was **29/35**. The experience developed my teamwork, communication and quality-review skills.

Tutor feedback recognised the technical methodology while recommending stronger business interpretation, clearer model justification and deeper critical evaluation. I will apply this feedback by connecting future model results more explicitly to practical decisions.

![Tutor Feedback](assets/Tutor%20Feedback.png)

*Figure 9. Tutor feedback.*

![Peer Evaluation](assets/Peer%20Evaluation.png)

*Figure 10. Peer self-evaluation.*

---

# 5. Neural Networks and Optimisation – Units 7–8

## Unit 7 – Perceptrons

The perceptron exercises covered Boolean AND classification, weighted inputs, biases and multilayer networks. I learned why single-layer perceptrons cannot represent every decision boundary.

![Perceptron Outputs](assets/Perceptron%20Outputs.png)

*Figure 11. Perceptron outputs.*

## Unit 8 – Gradient Descent

| Iterations | Learning Rate | Final Cost |
|---|---:|---:|
| 100 | 0.08 | 0.004121 |
| 100 | 0.01 | 0.480407 |
| 500 | 0.01 | 0.031985 |
| 100 | 0.10 | Approximately 5.97 × 10²⁸ |

The results demonstrated that inappropriate learning rates can cause divergence, while additional iterations may improve convergence.

![Gradient Descent Results 1](assets/Gradient%20Descent%20Results1.jpeg)

*Figure 12. Gradient-descent experiment.*

![Gradient Descent Results 2](assets/Gradient%20Descent%20Results2.jpeg)

*Figure 13. Additional optimisation results.*

## MovieLens Seminar

The MovieLens recommender activity produced an RMSE of **1.0400** and MAE of **0.8358**. It demonstrated the need to evaluate prediction error alongside practical recommendation quality.

![MovieLens Recommender Results](assets/MovieLens%20Recommender%20Results.png)

*Figure 14. Recommender-system results.*

---

# 6. CNN Activities – Units 9–10

The CNN exercises explored image classification and prediction confidence. The model correctly classified a car with **99.59% confidence**, but incorrectly identified a teacup as an airplane with **52.78% confidence**.

This highlighted the difference between confidence and correctness and encouraged more cautious interpretation of automated predictions.

![CNN Car Prediction](assets/CNN%20Car%20and%20Teacup%20Predictions.png)

*Figure 15. Correct car classification.*

![CNN Teacup Prediction](assets/CNN%20Car%20and%20Teacup%20Predictions1.png)

*Figure 16. Incorrect teacup classification.*


### CNN Layer Analysis and Critical Reflection

The Unit 10 activity explored how convolutional layers extract visual features and how ReLU introduces non-linearity. Intermediate feature maps illustrated the development of image representations.

The model correctly classified a car with 99.59% confidence but incorrectly classified a teacup as an airplane with 52.78% confidence. This highlighted the limitations of closed-set classification when an input does not belong to the model's known categories.

The activity demonstrated the importance of training-data coverage, cautious interpretation of confidence scores, and out-of-distribution detection in practical applications.


---

# 7. Unit 11 – Individual Pneumonia Project

The individual project compared HOG features with a Linear Support Vector Machine against a custom CNN using chest X-ray images (Mooney, 2018). The SVM approach builds on maximum-margin classification principles (Cortes and Vapnik, 1995).

The methodology included preprocessing, group-aware splitting, cross-validation and independent holdout evaluation involving **1,165 images**.

| Metric | HOG–SVM | CNN |
|---|---:|---:|
| Accuracy | **94.51%** | 91.93% |
| Sensitivity | **95.17%** | 91.17% |
| F1-score | **96.19%** | 94.28% |
| False negatives | **41** | 75 |

The classical model outperformed the CNN, demonstrating that architectural complexity does not guarantee stronger generalisation.

![Pneumonia Performance Comparison](assets/Pneumonia%20Performance%20Comparison%20and%20Confusion%20Matrices.png)

*Figure 17. Classification results and confusion matrices.*

Grad-CAM was used to investigate image regions associated with CNN predictions (Selvaraju et al., 2017). Some heatmaps suggested attention outside the lung fields, although these visualisations cannot establish causality.

![Grad-CAM Results](assets/Grad-CAM%20Results.png)

*Figure 18. Grad-CAM visualisations.*

The principal ethical concerns were false negatives, dataset representativeness, potential shortcut learning and patient safety. Neither experimental model should be considered clinically deployable without further validation and professional oversight.

## Evaluation in Relation to Unit 6

No separate Unit 6 proposal for the pneumonia project was available in the documented portfolio. Consequently, this comparison evaluates learning progression rather than claiming to assess an original proposal.

Unit 6 focused on business-oriented regression and clustering, while Unit 11 involved healthcare classification and greater attention to false negatives, explainability and generalisation.

The progression demonstrated that evaluation criteria must reflect the consequences of model errors. In healthcare, predictive performance must be interpreted alongside safety and clinical limitations.

---

# 8. Unit 11 – Model Performance Measurement

The performance-measurement activity investigated the influence of regularisation parameters on ROC-AUC and R².

Changing logistic-regression parameter C and ridge-regression parameter alpha demonstrated the importance of empirical hyperparameter evaluation.

![Unit 11 Performance Results](assets/Unit%2011%20Performance%20Results.png)

*Figure 19. Model-performance experiment.*

---

# 9. Collaborative Discussions

## Discussion 1 – Industry 4.0 and Industry 5.0

This discussion examined digital transformation, healthcare resilience and human oversight. The CrowdStrike disruption illustrated how technological failures can affect essential services.

The main learning outcome was that efficiency must be balanced against resilience, accountability and professional responsibility.

![Collaborative Discussion 1 Initial](assets/Collaborative%20Discussions%201%20initial.png)

*Figure 20. Initial discussion contribution.*

![Collaborative Discussion 1 Summary](assets/Collaborative%20Discussions%201%20summery.png)

*Figure 21. Discussion summary.*




### Peer Interaction Evidence

The following screenshot demonstrates my engagement with peers through constructive discussion and critical responses.

![Discussion 1 Peer Reply](assets/Discussion1-Peer-Reply.jpeg)

*My response to a peer in Collaborative Discussion 1.*



## Discussion 2 – AI Writers

The second discussion explored generative AI, authorship, misinformation and accountability.

I recognised that fluent AI-generated writing is not necessarily accurate and requires transparent use and human verification.

![Collaborative Discussion 2 Initial](assets/Collaborative%20Discussions%202%20initial.png)

*Figure 22. Initial discussion contribution.*

![Collaborative Discussion 2 Summary](assets/Collaborative%20Discussions%202%20summery.png)

*Figure 23. Discussion summary.*




### Peer Interaction Evidence

The following screenshot demonstrates my engagement with peers in the discussion of AI-assisted writing and professional responsibility.

![Discussion 2 Peer Reply](assets/Discussion2-Peer-Reply.jpeg)

*My response to a peer in Collaborative Discussion 2.*



---

# 10. Unit 12 – Future Machine Learning

Unit 12 introduced self-supervised learning, Neural Architecture Search, Edge AI and sustainable machine learning.

These developments offer opportunities for automation and efficient deployment but also create challenges involving privacy, computational cost and responsible governance.

![Unit 12 Evidence](assets/Unit%2012%20Evidence.png)

*Figure 24. Unit 12 evidence.*

---

# 11. Final Critical Reflection

This reflection uses the **WHAT, SO WHAT and NOW WHAT** framework developed by Rolfe, Freshwater and Jasper (2001).

## WHAT – Learning Experiences

At the beginning of the module, I understood machine learning mainly as the process of selecting algorithms, training models and measuring accuracy. I expected technical performance to be the principal indicator of success. However, the practical exercises, collaborative activities and assessments progressively challenged this assumption.

The early Auto-MPG activity demonstrated that missing values and feature relationships must be examined before modelling. Regression exercises showed that statistical association does not automatically establish causation or reliable prediction. The Jaccard and clustering activities introduced another challenge: results depend on how observations are represented and how algorithms define similarity.

The gradient-descent experiment was particularly useful because changing a single parameter produced dramatically different outcomes. A learning rate of 0.08 produced a low final cost, whereas 0.10 caused divergence. This demonstrated the practical consequences of hyperparameter selection.

The CNN exercises also exposed a limitation of model confidence. Although the classifier recognised a car correctly, it misclassified a teacup as an airplane. This experience prepared me to question model outputs rather than accept confidence scores without investigation.

Two assessments were especially influential: the Unit 6 Airbnb group project and the Unit 11 individual pneumonia classification project. Together, they provided contrasting business and healthcare contexts in which to apply and evaluate machine-learning techniques.

## SO WHAT – Critical Analysis

The Airbnb project demonstrated that achieving a relatively strong overall regression result does not mean a model performs equally well for every observation. Tuned XGBoost achieved an R² of 0.623, but prediction errors for expensive listings remained problematic.

This made me reconsider the relationship between model metrics and business value. A model may outperform alternatives statistically while still producing recommendations that require caution. Tutor feedback reinforced this point by identifying opportunities to strengthen business interpretation, model justification and critical evaluation.

My individual contribution involved completing my assigned part of the project and reviewing the complete research report. Reviewing the full document helped me see the importance of consistency between methodology, results and conclusions. However, I also recognised that effective teamwork requires more than completing allocated tasks. Clear communication, documented responsibilities and regular progress reviews are essential for producing an integrated submission.

My self-evaluation score of 29/35 encouraged me to reflect on how I could contribute more effectively to future virtual teams. In particular, I would benefit from more structured checkpoints and earlier discussion of how individual sections connect to the overall research question.

The pneumonia project challenged a different assumption: that a CNN should necessarily outperform a classical model on an image-classification problem.

The HOG–SVM achieved 94.51% accuracy compared with 91.93% for the CNN. More importantly, it produced 41 false negatives rather than 75. These findings demonstrated that greater complexity does not guarantee better generalisation and that evaluation should account for the practical consequences of errors.

In a healthcare application, missing a positive case may have serious implications. Therefore, overall accuracy alone is insufficient. Sensitivity, false negatives, dataset representativeness and independent validation must be considered together.

Grad-CAM introduced an additional dimension to this analysis. The visualisations suggested that some predictions might be influenced by image regions outside the lungs. However, I learned that visual explanations do not prove the causal basis of predictions. This distinction is important because apparently convincing visualisations may create unwarranted confidence in a model.

The collaborative discussions broadened my understanding of professional responsibility. The discussion of Industry 4.0 and Industry 5.0 highlighted resilience and human oversight, while the AI-writing discussion raised questions about transparency, authorship and misinformation.

These activities helped me recognise that machine-learning professionals are responsible not only for technical development but also for explaining limitations and anticipating possible harm.

Overall, the module changed my understanding of model quality. I now view successful machine learning as a balance between predictive performance, trustworthy evaluation, interpretability, communication and ethical responsibility.

## NOW WHAT – Professional Development

In future projects, I will begin by defining the practical problem and evaluation criteria before selecting algorithms. I will assess dataset quality, identify possible sources of bias or leakage, and establish a transparent baseline before experimenting with more complex methods.

I will also maintain a reproducible experiment log recording preprocessing choices, data splits, hyperparameters and evaluation results. This will help me explain why a model was selected and support more reliable comparisons.

For higher-risk applications, particularly healthcare, I will place greater emphasis on sensitivity, subgroup performance, external validation and uncertainty. I will avoid treating experimental accuracy as evidence that a system is ready for real-world deployment.

The Airbnb feedback also identified a professional development priority: communicating technical findings in a way that supports decisions. I intend to improve how I explain business implications, assumptions and limitations to non-technical stakeholders.

In future group projects, I will clarify responsibilities earlier, participate in regular progress reviews and document my individual contribution more explicitly. I will also review the complete final submission to check whether its sections form a coherent argument.

My short-term goal is to improve reproducibility and technical documentation. My medium-term goal is to develop stronger skills in explainable AI and model evaluation. My longer-term goal is to apply these practices in responsible professional machine-learning projects.

The most significant lesson from this module is that choosing the model with the highest reported score is not enough. Reliable machine learning requires critical judgement throughout the entire process, from defining the problem and preparing data to evaluating results and communicating their consequences.

---

# 12. Professional Skills and Development Plan

| Skill | Evidence | Development Priority |
|---|---|---|
| Data analysis | Auto-MPG, Airbnb | Data auditing |
| Programming | Python, SVM, CNN | Reproducibility |
| Critical evaluation | Pneumonia comparison | External validation |
| Problem solving | Gradient descent | Experiment tracking |
| Teamwork | Airbnb project | Progress reviews |
| Communication | Discussions, feedback | Stakeholder reporting |
| Ethics | Medical imaging, AI writing | Responsible AI |

**Short term:** Improve experiment documentation and reproducibility.

**Medium term:** Develop explainable AI and advanced validation skills.

**Long term:** Apply responsible machine-learning practices in professional projects.

---

# References

Breiman, L. (2001) ‘Random forests’, *Machine Learning*, 45(1), pp. 5–32. https://doi.org/10.1023/A:1010933404324

Chen, T. and Guestrin, C. (2016) ‘XGBoost: A scalable tree boosting system’, *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, pp. 785–794. https://doi.org/10.1145/2939672.2939785

Cortes, C. and Vapnik, V. (1995) ‘Support-vector networks’, *Machine Learning*, 20, pp. 273–297. https://doi.org/10.1007/BF00994018

Dgomonov (2019) *New York City Airbnb Open Data*. Kaggle. Available at: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

Mooney, P. (2018) *Chest X-Ray Images (Pneumonia)*. Kaggle. Available at: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

Rolfe, G., Freshwater, D. and Jasper, M. (2001) *Critical Reflection in Nursing and the Helping Professions: A User's Guide*. Basingstoke: Palgrave Macmillan.

Rousseeuw, P.J. (1987) ‘Silhouettes: A graphical aid to the interpretation and validation of cluster analysis’, *Journal of Computational and Applied Mathematics*, 20, pp. 53–65. https://doi.org/10.1016/0377-0426(87)90125-7

Selvaraju, R.R. et al. (2017) ‘Grad-CAM: Visual explanations from deep networks via gradient-based localization’, *Proceedings of the IEEE International Conference on Computer Vision*, pp. 618–626. https://doi.org/10.1109/ICCV.2017.74
