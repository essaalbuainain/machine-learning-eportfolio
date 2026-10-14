
# Machine Learning – ML_PCOM7E e-Portfolio

**Student Name:** Essa Albuainain  
**Institution:** University of Essex Online  
**Module:** Machine Learning (ML_PCOM7E)  
**Assessment:** Individual e-Portfolio  
**Portfolio:** https://essaalbuainain.github.io/machine-learning-eportfolio/

---

## Introduction and Learning Outcomes

This e-Portfolio documents my learning across Units 1–12 through practical exercises, collaborative discussions, tutor feedback, group and individual assessments, and critical reflection.

It addresses ethical and professional responsibility, dataset suitability, application and evaluation of machine-learning methods, and effective virtual teamwork.

My development progressed from exploratory analysis and regression to clustering, neural networks, model evaluation, explainability and responsible AI.

---

# 1. Foundations – Units 1–3

## Unit 1 – Machine Learning Principles

Unit 1 introduced supervised and unsupervised learning, algorithm selection and the machine-learning lifecycle. I learned that reliable modelling begins with defining the problem and understanding available data.

## Unit 2 – Exploratory Data Analysis

The Auto-MPG activity identified six missing horsepower values and negative correlations between MPG and vehicle weight, displacement and cylinders.

This demonstrated the importance of investigating missing data and feature relationships before modelling. Correlation does not establish causation.

![Auto-MPG Correlation Heatmap](assets/Auto-MPG%20Correlation%20Heatmap.jpeg)

*Figure 1. Auto-MPG correlation analysis.*

## Unit 3 – Correlation and Regression

I investigated covariance, Pearson correlation, linear regression and polynomial regression. These methods demonstrated how assumptions and model complexity influence fitted relationships and overfitting risk.

![Correlation and Regression Results](assets/Correlation%20and%20Regression%20Results.jpg)

*Figure 2. Correlation and regression results.*

---

# 2. Applied Regression – Unit 4

The exercises investigated fuel-consumption relationships and population–GDP indicators from 2001 to 2021.

The regression illustrated that a single predictor cannot necessarily explain complex economic outcomes. I learned to distinguish statistical association from reliable prediction.

![Population GDP Regression](assets/Population%E2%80%93GDP%20Regression.png)

*Figure 3. Population–GDP regression.*

---

# 3. Similarity and Clustering – Units 5–6

## Unit 5 – Jaccard Distance

The categorical similarity exercise produced:

| Comparison | Distance |
|---|---:|
| Jack–Mary | 0.7273 |
| Jack–Jim | 0.4444 |
| Jim–Mary | 0.9231 |

Jack and Jim were the most similar pair, demonstrating how similarity depends on attribute representation.

![Jaccard Calculations](assets/Jaccard%20Calculations.png)

*Figure 4. Jaccard calculations.*

## Unit 5 – K-Means Wiki

The wiki explored centroid initialisation, iterative assignment and cluster interpretation. Generated clusters require validation; silhouette analysis offers one possible measure (Rousseeuw, 1987).

![K-Means Wiki](assets/Wiki%20.jpeg)

*Figure 5. K-Means wiki evidence.*

## Unit 6 – Iris Clustering

I applied K-Means with three clusters to Iris data. This illustrated why unsupervised assignments should not automatically be interpreted as known classification labels.

![Iris Clustering](assets/Iris%20Clustering.png)

*Figure 6. Iris clustering.*

---

# 4. Unit 6 Group Project – Airbnb NYC

The group investigated Airbnb listing-price prediction and supply segmentation using New York City Airbnb Open Data (Dgomonov, 2019).

We compared Linear Regression, Random Forest (Breiman, 2001) and XGBoost (Chen and Guestrin, 2016).

| Model | R² |
|---|---:|
| Linear Regression | 0.501 |
| Tuned Random Forest | 0.608 |
| Untuned XGBoost | 0.617 |
| Tuned XGBoost | **0.623** |

Although tuned XGBoost performed best, errors for expensive listings limited the reliability of some recommendations.

![Airbnb Model Comparison](assets/Airbnb%20Model%20Comparison%20and%20Segmentation2.png)

*Figure 7. Regression model comparison.*

K-Means identified four supply-side segments: high-turnover performers, listed-but-not-booking properties, commercial operators and dormant hosts.

![Airbnb Supply Segmentation](assets/Airbnb%20Model%20Comparison%20and%20Segmentation1.png)

*Figure 8. Airbnb supply segmentation.*

## Individual Contribution and Feedback

I completed my assigned part of the group project and reviewed the full research report for consistency, quality and presentation before submission.

Reviewing the complete work strengthened my understanding of how individual contributions form a coherent investigation.

My peer self-evaluation was **29/35**. Tutor feedback recognised the methodology but recommended stronger business interpretation, model justification and critical evaluation.

![Tutor Feedback](assets/Tutor%20Feedback.png)

*Figure 9. Tutor feedback.*

![Peer Evaluation](assets/Peer%20Evaluation.png)

*Figure 10. Peer self-evaluation.*

---

# 5. Neural Networks and Optimisation – Units 7–8

## Unit 7 – Perceptrons

The activities investigated weighted inputs, biases, Boolean AND classification and multilayer networks. I learned why single-layer perceptrons cannot represent every decision boundary.

![Perceptron Outputs](assets/Perceptron%20Outputs.png)

*Figure 11. Perceptron outputs.*

## Unit 8 – Gradient Descent

| Iterations | Learning Rate | Final Cost |
|---|---:|---:|
| 100 | 0.08 | 0.004121 |
| 100 | 0.01 | 0.480407 |
| 500 | 0.01 | 0.031985 |
| 100 | 0.10 | Approximately 5.97 × 10²⁸ |

The results demonstrated that unsuitable learning rates can cause divergence, while additional iterations may improve convergence.

![Gradient Descent Results 1](assets/Gradient%20Descent%20Results1.jpeg)

*Figure 12. Gradient-descent experiment.*

![Gradient Descent Results 2](assets/Gradient%20Descent%20Results2.jpeg)

*Figure 13. Additional optimisation results.*

## MovieLens Seminar

The recommender-system exercise produced RMSE **1.0400** and MAE **0.8358**, highlighting the importance of evaluating prediction error alongside recommendation quality.

![MovieLens Recommender Results](assets/MovieLens%20Recommender%20Results.png)

*Figure 14. MovieLens results.*

---

# 6. CNN Activities – Units 9–10

## Unit 9 – CNN Object Recognition

The activity explored image classification and prediction confidence. The saved notebook also includes selecting a test image using `x_test[7]`. However, the available evidence does not establish a separate prediction result for a modified `x_test[16]` experiment.

![CNN Car Prediction](assets/CNN%20Car%20and%20Teacup%20Predictions.png)

*Figure 15. Correct car classification.*

![CNN Teacup Prediction](assets/CNN%20Car%20and%20Teacup%20Predictions1.png)

*Figure 16. Incorrect teacup classification.*

### Ethical and Professional Reflection

Image classifiers may produce confident but incorrect predictions, especially when inputs differ from training examples. Responsible use requires recognising dataset limitations, assessing unexpected predictions and avoiding unsupported claims of reliability. Human oversight is particularly important when classification errors could affect safety or important decisions.

## Unit 10 – CNN Layer Analysis and Critical Reflection

Convolutional layers extract visual patterns, while ReLU introduces non-linearity by setting negative activations to zero. Intermediate feature maps illustrate how representations change across successive layers.

![Intermediate CNN Feature Maps](assets/Unit10_Intermediate_Feature_Maps_1.png)

*Figure 17. Intermediate CNN feature maps illustrating learned visual representations.*

![Additional CNN Feature Maps](assets/Unit10_Intermediate_Feature_Maps_2.png)

*Figure 18. Feature maps from a subsequent convolutional layer.*

The intermediate feature maps provided insight into how the CNN processes visual information through successive layers. Earlier convolutional layers respond to relatively simple patterns, while deeper layers can represent more complex combinations of visual features.

ReLU enables the network to learn non-linear relationships. However, feature maps show layer responses to an input image; they do not independently establish why a particular classification decision was made.

The model correctly classified a car with **99.59% confidence** but incorrectly classified a teacup as an airplane with **52.78% confidence**.

This demonstrated that feature extraction does not guarantee reliable recognition. Closed-set classifiers may assign unfamiliar inputs to known categories, highlighting the importance of training-data coverage and out-of-distribution detection.

---

# 7. Unit 11 – Individual Pneumonia Project

The project compared HOG features with a Linear Support Vector Machine against a custom CNN using chest X-ray images (Mooney, 2018). The SVM approach builds on maximum-margin classification (Cortes and Vapnik, 1995).

The methodology included preprocessing, group-aware splitting, cross-validation and an independent holdout of **1,165 images**.

| Metric | HOG–SVM | CNN |
|---|---:|---:|
| Accuracy | **94.51%** | 91.93% |
| Sensitivity | **95.17%** | 91.17% |
| F1-score | **96.19%** | 94.28% |
| False negatives | **41** | 75 |

The classical model performed better, demonstrating that greater complexity does not guarantee stronger generalisation.

![Pneumonia Performance Comparison](assets/Pneumonia%20Performance%20Comparison%20and%20Confusion%20Matrices.png)

*Figure 19. Performance comparison and confusion matrices.*

Grad-CAM examined CNN predictions (Selvaraju et al., 2017). Some heatmaps suggested attention outside the lung fields, but these visualisations cannot establish causality.

![Grad-CAM Results](assets/Grad-CAM%20Results.png)

*Figure 20. Grad-CAM visualisations.*

False negatives, shortcut learning, dataset representativeness and patient safety were major concerns. Neither experimental model is ready for autonomous clinical deployment without further validation.

## Evaluation in Relation to Unit 6

No separate Unit 6 proposal for pneumonia was available in the documented portfolio. This comparison therefore evaluates learning progression rather than claiming to assess an original proposal.

Unit 6 focused on business regression and clustering, while Unit 11 required healthcare classification, sensitivity analysis and explainability. The progression demonstrated that evaluation criteria must reflect application-specific consequences.

---

# 8. Unit 11 – Model Performance Measurement

The activity investigated how regularisation affects classification and regression performance using scikit-learn (Pedregosa et al., 2011).

## Logistic Regression – Effect of C

The breast-cancer dataset produced:

| C | ROC-AUC |
|---:|---:|
| 0.001 | 0.990356 |
| 0.01 | 0.995178 |
| 0.1 | 0.997065 |
| 1 | **0.997694** |
| 10 | 0.994549 |
| 100 | 0.983648 |

C = 1 achieved the highest AUC among tested values. Increasing C further reduced performance, demonstrating that weaker regularisation does not necessarily improve generalisation.

## Ridge Regression – Effect of Alpha

The diabetes dataset produced:

| Alpha | R² |
|---:|---:|
| 0 | 0.484906 |
| 0.01 | 0.484921 |
| 0.1 | 0.485049 |
| 1 | 0.485896 |
| 10 | 0.488092 |
| 100 | **0.490477** |

R² improved modestly across the tested alpha values. Alpha = 100 performed best within this experiment, although additional testing would be required to identify an optimal value.

![Unit 11 Performance Results](assets/Unit%2011%20Performance%20Results.png)

*Figure 21. Regularisation experiments and performance results.*

---

# 9. Collaborative Discussions

## Discussion 1 – Industry 4.0 and Industry 5.0

The discussion examined digital transformation, healthcare resilience and human oversight. The CrowdStrike disruption illustrated how digital-system failures can affect essential services.

I learned that technological efficiency must be balanced with resilience, accountability and professional responsibility.

![Discussion 1 Initial](assets/Collaborative%20Discussions%201%20initial.png)

*Figure 22. Initial discussion contribution.*

![Discussion 1 Summary](assets/Collaborative%20Discussions%201%20summery.png)

*Figure 23. Discussion summary.*

### Peer Interaction Evidence

The following screenshots document my participation in discussions with peers.

![Discussion 1 First Reply](assets/Discussion1-Peer-Reply.jpeg)

*Figure 24. First peer response in Discussion 1.*

![Discussion 1 Second Reply](assets/Discussion1-Peer-Reply2.jpeg)

*Figure 25. Second peer response in Discussion 1.*

## Discussion 2 – AI Writers

The discussion examined AI-generated writing, authorship, reliability and accountability.

Generative AI can improve performance on certain writing tasks (Noy and Zhang, 2023), while potentially reducing the collective diversity of creative outputs (Doshi and Hauser, 2024).

These findings suggest that productivity benefits must be considered alongside accuracy, transparency, originality and human responsibility.

![Discussion 2 Initial](assets/Collaborative%20Discussions%202%20initial.png)

*Figure 26. Initial discussion contribution.*

![Discussion 2 Summary](assets/Collaborative%20Discussions%202%20summery.png)

*Figure 27. Discussion summary.*

### Peer Interaction Evidence

The screenshots provide evidence of my engagement with other participants.

![Discussion 2 First Reply](assets/Discussion2-Peer-Reply.jpeg)

*Figure 28. First peer response in Discussion 2.*

![Discussion 2 Second Reply](assets/Discussion2-Peer-Reply2.jpeg)

*Figure 29. Second peer response in Discussion 2.*

---

# 10. Unit 12 – Future Machine Learning

Unit 12 explored self-supervised learning, Neural Architecture Search, Edge AI and sustainable machine learning.

These approaches offer opportunities for efficient deployment but introduce challenges involving privacy, computational resources and responsible governance.

![Unit 12 Evidence](assets/Unit%2012%20Evidence.png)

*Figure 30. Unit 12 learning evidence.*

---

# 11. Final Critical Reflection

This reflection follows the **What? So What? Now What?** framework (Rolfe, Freshwater and Jasper, 2001).

## WHAT – Learning Experiences

At the beginning of the module, I mainly understood machine learning as selecting algorithms, training models and comparing accuracy. I expected technical performance to be the primary indicator of success. However, the twelve units demonstrated that reliable outcomes also depend on data quality, evaluation methods, interpretability and professional judgement.

The Auto-MPG exercise showed why missing values and feature relationships must be investigated before modelling. Regression and clustering activities highlighted how assumptions and data representation influence results. The Jaccard exercise demonstrated that similarity depends on selected attributes.

Gradient descent was particularly useful because a small change in learning rate produced dramatically different outcomes. A learning rate of 0.08 achieved a low final cost, whereas 0.10 caused divergence. This demonstrated the importance of understanding optimisation rather than simply running an algorithm.

The CNN activities challenged my understanding of prediction confidence. Although the model correctly recognised a car, it misclassified a teacup as an airplane. Examining intermediate feature maps helped me understand how convolutional layers represent visual information without guaranteeing correct predictions.

Two assessments were particularly influential: the Unit 6 Airbnb group project and the Unit 11 pneumonia detection project. They provided different business and healthcare contexts for evaluating machine-learning decisions.

## SO WHAT – Critical Evaluation

The Airbnb project demonstrated that strong aggregate performance does not guarantee equally reliable predictions across all observations. Tuned XGBoost achieved an R² of 0.623, but errors for expensive listings remained substantial. This challenged my assumption that the best overall metric automatically identifies the most useful business model.

Tutor feedback reinforced the importance of translating analytical findings into practical recommendations. Although the project demonstrated technical strengths, the feedback identified opportunities to improve model justification, business interpretation and critical discussion of limitations.

My individual contribution involved completing my assigned section and reviewing the entire research report before submission. This helped me understand how separate contributions must form a coherent investigation. However, I recognised that completing assigned work alone is insufficient without communication, coordination and collective review.

My peer self-evaluation score of 29/35 reflected positive participation while encouraging me to improve preparation and collaboration. In future group projects, I need to clarify responsibilities earlier and establish regular checkpoints.

The pneumonia project challenged another assumption: that deep learning would necessarily outperform classical machine learning in image classification.

The HOG–SVM achieved 94.51% accuracy compared with 91.93% for the CNN. More importantly, it produced 41 false negatives rather than 75. These results demonstrated that architectural complexity does not guarantee better generalisation and that the significance of errors depends on the application.

In healthcare, missed positive cases may delay clinical investigation. Therefore, sensitivity and false-negative counts can be particularly important. However, strong performance on one dataset cannot establish clinical readiness.

Grad-CAM introduced another limitation. Some visualisations suggested that the CNN might attend to regions outside the lungs, raising concerns about shortcut learning. Nevertheless, attention maps do not prove the causal basis of a prediction. This showed me why explainability techniques require cautious interpretation and additional testing (Selvaraju et al., 2017).

The project also exposed limitations in fairness evaluation. Without reliable demographic information, meaningful comparisons across patient groups were not possible. I learned that acknowledging missing evidence is more responsible than making unsupported claims about equitable performance.

Collaborative discussions broadened my understanding of ethical and professional responsibilities. The healthcare digital-transformation discussion highlighted resilience and human oversight. The AI-writing discussion raised questions about misinformation, authorship and transparency. Research on generative AI also demonstrated that individual productivity and collective creativity may be affected differently (Noy and Zhang, 2023; Doshi and Hauser, 2024).

The Unit 11 regularisation activity reinforced the importance of testing assumptions empirically. Changes to C and alpha produced measurable differences in AUC and R², demonstrating that parameter selection requires evidence rather than intuition.

Overall, I progressed from reporting model results to questioning their reliability, limitations and consequences. I now understand successful machine learning as a balance between predictive performance, trustworthy evaluation, communication and ethical responsibility.

## NOW WHAT – Professional Development

My first priority is to strengthen reproducible machine-learning practice. In future projects, I will document dataset sources, preprocessing choices, data splits, hyperparameters and evaluation procedures. I will establish baseline models before experimenting with more complex architectures.

I also intend to develop stronger skills in model calibration, fairness assessment and external validation, particularly for higher-risk applications. Where demographic or clinical information is unavailable, I will acknowledge the limitation rather than claim that a model is fair or suitable for deployment.

Another priority is communicating results more effectively to non-technical stakeholders. The Airbnb feedback demonstrated that analytical reports must explain the practical significance of findings, not merely present metrics. I will therefore make assumptions, uncertainty and recommendations more explicit.

For future group projects, I will establish regular checkpoints, document my individual responsibilities and continue reviewing complete submissions for consistency between objectives, methods, results and conclusions.

My short-term goal is to improve reproducibility and experiment tracking. My medium-term goal is to develop advanced evaluation and explainability skills. My longer-term goal is to apply responsible machine-learning principles in professional projects.

The most significant lesson from this module is that choosing the model with the highest reported score is insufficient. Responsible machine learning requires critical judgement throughout the workflow, from data preparation and modelling to interpretation, communication and accountability.

---

# 12. Professional Skills and Development Plan

| Skill | Evidence | Development Priority |
|---|---|---|
| Data analysis | Auto-MPG, Airbnb | Data auditing |
| Programming | Python, SVM, CNN | Reproducibility |
| Critical evaluation | Pneumonia project | External validation |
| Optimisation | Gradient descent, regularisation | Experiment tracking |
| Teamwork | Airbnb group project | Regular checkpoints |
| Communication | Discussions and tutor feedback | Stakeholder reporting |
| Ethics | Medical imaging, AI writing | Responsible AI |

**Short term:** Improve experiment documentation.

**Medium term:** Develop explainability and validation skills.

**Long term:** Apply responsible machine learning professionally.

---

# References

Breiman, L. (2001) ‘Random forests’, *Machine Learning*, 45(1), pp. 5–32. https://doi.org/10.1023/A:1010933404324

Chen, T. and Guestrin, C. (2016) ‘XGBoost: A scalable tree boosting system’, *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, pp. 785–794. https://doi.org/10.1145/2939672.2939785

Cortes, C. and Vapnik, V. (1995) ‘Support-vector networks’, *Machine Learning*, 20, pp. 273–297. https://doi.org/10.1007/BF00994018

Dgomonov (2019) *New York City Airbnb Open Data*. Kaggle. Available at: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

Doshi, A.R. and Hauser, O.P. (2024) ‘Generative AI enhances individual creativity but reduces the collective diversity of novel content’, *Science Advances*, 10(28), eadn5290. https://doi.org/10.1126/sciadv.adn5290

Mooney, P. (2018) *Chest X-Ray Images (Pneumonia)*. Kaggle. Available at: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

Noy, S. and Zhang, W. (2023) ‘Experimental evidence on the productivity effects of generative artificial intelligence’, *Science*, 381(6654), pp. 187–192. https://doi.org/10.1126/science.adh2586

Pedregosa, F. et al. (2011) ‘Scikit-learn: Machine learning in Python’, *Journal of Machine Learning Research*, 12, pp. 2825–2830. Available at: https://jmlr.org/papers/v12/pedregosa11a.html

Rolfe, G., Freshwater, D. and Jasper, M. (2001) *Critical Reflection in Nursing and the Helping Professions: A User's Guide*. Basingstoke: Palgrave Macmillan.

Rousseeuw, P.J. (1987) ‘Silhouettes: A graphical aid to the interpretation and validation of cluster analysis’, *Journal of Computational and Applied Mathematics*, 20, pp. 53–65. https://doi.org/10.1016/0377-0426(87)90125-7

Selvaraju, R.R. et al. (2017) ‘Grad-CAM: Visual explanations from deep networks via gradient-based localization’, *Proceedings of the IEEE International Conference on Computer Vision*, pp. 618–626. https://doi.org/10.1109/ICCV.2017.74
