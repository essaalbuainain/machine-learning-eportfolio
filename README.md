
# Machine Learning – ML_PCOM7E e-Portfolio

**Student Name:** Essa Albuainain  
**Module:** Machine Learning (ML_PCOM7E)  
**Institution:** University of Essex Online  
**Assessment:** Individual e-Portfolio  
**Published e-Portfolio:** https://essaalbuainain.github.io/machine-learning-eportfolio/

---

## About This e-Portfolio

This e-Portfolio documents my learning and professional development throughout the Machine Learning module. It brings together practical exercises, collaborative discussions, seminar activities, group and individual projects, tutor feedback, and critical reflection.

My learning progressed from exploratory data analysis and regression to clustering, neural networks, model optimisation, explainable AI, and responsible machine-learning practice.

Two major projects provided opportunities to apply these skills:

- **Unit 6 Group Project:** Airbnb NYC Price Prediction and Supply Segmentation.
- **Unit 11 Individual Project:** Pneumonia Detection Using HOG + Linear SVM and a Custom CNN.

The portfolio demonstrates that successful machine learning requires more than strong predictive performance. Data quality, model limitations, interpretability, professional responsibility, and effective communication are equally important.

---

## Learning Outcomes

| Learning Outcome | Portfolio Evidence |
|---|---|
| **LO1 – Legal, social, ethical and professional issues** | Collaborative discussions, medical imaging, CNN ethics, and responsible AI |
| **LO2 – Dataset suitability and limitations** | Auto-MPG analysis, regression, Airbnb data preparation, and medical-image evaluation |
| **LO3 – Application and critical evaluation of machine-learning techniques** | Regression, Jaccard distance, K-Means, neural networks, optimisation, recommender systems, and pneumonia classification |
| **LO4 – Effective virtual teamwork** | Airbnb group assessment, tutor feedback, peer evaluation, and collaborative discussions |

---

# 1. Foundations of Machine Learning – Units 1–3

The opening units developed my understanding of machine-learning principles and the importance of examining data before selecting an algorithm.

I learned that model selection should depend on the problem, the available observations, the quality of the data, and the assumptions underlying each technique.

## Unit 2 – Exploratory Data Analysis

The Auto-MPG exercise involved examining missing values, distributions, correlations, and relationships between vehicle characteristics.

Six missing horsepower observations were identified. The analysis also showed strong negative correlations between MPG and vehicle weight, displacement, and cylinders.

This demonstrated how exploratory data analysis can identify potential predictors and data-quality concerns before modelling.

However, I also learned that correlation does not establish causation.

![Auto-MPG Correlation Heatmap](assets/Auto-MPG%20Correlation%20Heatmap.jpeg)

*Figure 1. Auto-MPG correlation heatmap showing relationships between fuel efficiency and vehicle characteristics.*

## Unit 3 – Correlation and Regression

The practical activities introduced covariance, Pearson correlation, simple linear regression, multiple linear regression, and polynomial regression.

Comparing these techniques helped me understand how model assumptions and complexity influence fitted relationships.

An important lesson was that a more flexible model can capture nonlinear patterns but may also increase the risk of overfitting.

![Correlation and Regression Results](assets/Correlation%20and%20Regression%20Results.jpg)

*Figure 2. Correlation and regression practical results.*

---

# 2. Applied Regression – Unit 4

Unit 4 extended regression analysis to fuel-consumption data and an investigation involving population and GDP-related indicators from 2001 to 2021.

The activity involved examining associations, plotting observations, and interpreting a fitted regression line.

The substantial variation around the fitted relationship demonstrated the limitations of using a single predictor to explain complex economic outcomes.

I learned to distinguish between identifying an association and developing a model that is sufficiently reliable for practical decisions.

![Population GDP Regression](assets/Population%E2%80%93GDP%20Regression.png)

*Figure 3. Population and GDP-related regression analysis.*

---

# 3. Similarity Measures and Clustering – Units 5–6

## Unit 5 – Jaccard Distance

The Jaccard activity compared categorical observations for Jack, Mary, and Jim.

The calculated distances were:

| Comparison | Jaccard Distance |
|---|---:|
| Jack and Mary | 0.7273 |
| Jack and Jim | 0.4444 |
| Jim and Mary | 0.9231 |

Jack and Jim were the most similar pair under the representation used.

This activity demonstrated that the representation of categorical attributes influences the resulting similarity measures.

![Jaccard Calculations](assets/Jaccard%20Calculations.png)

*Figure 4. Jaccard distance calculations.*

## Unit 5 – K-Means Wiki Activity

The K-Means wiki activity explored iterative cluster assignment and centroid updates.

The animations demonstrated how the initial positions of centroids can influence the final clustering outcome.

I learned that clustering algorithms can produce groups even when those groups do not necessarily represent meaningful natural categories. Cluster quality therefore requires interpretation and, where appropriate, validation measures such as silhouette analysis (Rousseeuw, 1987).

This reinforced the importance of interpreting and validating clustering results.

![K-Means Wiki](assets/Wiki%20.jpeg)

*Figure 5. Unit 5 K-Means wiki activity.*

## Unit 6 – Iris Clustering

The Iris exercise applied K-Means with three clusters.

This helped me understand the distinction between unsupervised clustering and supervised classification.

Cluster labels are algorithmically assigned and do not necessarily correspond directly to known biological categories.

![Iris Clustering](assets/Iris%20Clustering.png)

*Figure 6. Iris dataset clustering using K-Means.*

---

# 4. Unit 6 Group Project – Airbnb NYC

## Project Overview

The group project investigated Airbnb NYC price prediction and supply segmentation using classical machine-learning techniques.

The analysis used the New York City Airbnb Open Data dataset (Dgomonov, 2019) and combined supervised regression with unsupervised clustering.

The main objectives were to predict listing prices and identify meaningful supply-side patterns.

## Regression Model Comparison

The project compared Linear Regression, Random Forest, and XGBoost. Random forests aggregate predictions from multiple decision trees (Breiman, 2001), while XGBoost uses scalable gradient-boosted trees (Chen and Guestrin, 2016).

| Model | R² |
|---|---:|
| Linear Regression | 0.501 |
| Tuned Random Forest | 0.608 |
| Untuned XGBoost | 0.617 |
| Tuned XGBoost | **0.623** |

Tuned XGBoost achieved the strongest overall performance.

However, prediction errors remained substantial for expensive listings. This showed that aggregate performance metrics should not be interpreted without considering variation across different price categories.

![Airbnb Model Comparison](assets/Airbnb%20Model%20Comparison%20and%20Segmentation2.png)

*Figure 7. Regression model comparison for Airbnb price prediction.*

## Airbnb Supply Segmentation

K-Means identified four supply-side segments:

1. High-turnover performers.
2. Listed-but-not-booking properties.
3. Commercial operators.
4. Dormant hosts.

The project distinguished supply segmentation from customer segmentation because the dataset described listings and hosts rather than individual guests.

The findings suggested opportunities for targeted pricing support, although the limitations of the available data reduced the certainty of business recommendations.

![Airbnb Supply Segmentation](assets/Airbnb%20Model%20Comparison%20and%20Segmentation1.png)

*Figure 8. Four Airbnb supply-side segments.*

## Tutor Feedback

Tutor feedback recognised the methodology, data preparation, feature engineering, model comparison, and visual presentation.

Areas identified for improvement included stronger business interpretation, clearer justification of model selection, more critical discussion of limitations, and more developed interpretation of the clusters.

This feedback demonstrated that technical accuracy must be accompanied by practical relevance and clear communication.

![Tutor Feedback](assets/Tutor%20Feedback.png)

*Figure 9. Tutor feedback on the Airbnb group assessment.*

## Teamwork and Individual Contribution

The project developed my experience of virtual collaboration, task allocation, coordination, and collective review. The portfolio includes a personal peer self-evaluation and tutor feedback as evidence of participation; however, the available material does not establish a detailed, individually attributable task log. Any account of specific coding, analysis or presentation responsibilities should be added only after checking the original group records.

My self-evaluation score was **29/35**.

The experience highlighted strengths in initiative and task completion, while also identifying opportunities to improve meeting preparation, communication, and shared review.

I learned that effective virtual teamwork requires clear responsibilities, regular checkpoints, and collective accountability.

![Peer Evaluation](assets/Peer%20Evaluation.png)

*Figure 10. Personal peer self-evaluation.*

---

# 5. Neural Networks and Optimisation – Units 7–8

## Unit 7 – Perceptron Exercises

Unit 7 introduced perceptrons, Boolean AND classification, and multilayer neural networks using sigmoid activation.

The practical exercises demonstrated how weighted inputs, biases, and activation functions influence classification.

I also learned why simple perceptrons cannot solve every classification problem and why multilayer architectures are necessary for more complex relationships.

![Perceptron Outputs](assets/Perceptron%20Outputs.png)

*Figure 11. Perceptron classification outputs.*

## Unit 8 – Gradient Descent

The gradient-descent activity investigated the effects of learning rate and iteration count.

| Iterations | Learning Rate | Final Cost |
|---|---:|---:|
| 100 | 0.08 | 0.004121 |
| 100 | 0.01 | 0.480407 |
| 500 | 0.01 | 0.031985 |
| 100 | 0.10 | Approximately 5.97 × 10²⁸ |

A moderate learning rate produced rapid improvement, while a larger learning rate caused divergence.

This demonstrated that optimisation depends on appropriate hyperparameter selection and monitoring.

![Gradient Descent Results 1](assets/Gradient%20Descent%20Results1.jpeg)

*Figure 12. Gradient-descent experiment showing optimisation behaviour.*

![Gradient Descent Results 2](assets/Gradient%20Descent%20Results2.jpeg)

*Figure 13. Additional gradient-descent results illustrating the influence of parameter selection.*

## Unit 8 Seminar – MovieLens Recommender

The seminar explored recommendation systems, collaborative filtering, matrix factorisation, and evaluation.

The MovieLens 100K activity produced the following results for the matrix-factorisation model:

| Metric | Result |
|---|---:|
| RMSE | 1.0400 |
| MAE | 0.8358 |

This demonstrated the importance of evaluating recommendation quality rather than assuming that low prediction error automatically guarantees useful recommendations.

![MovieLens Recommender Results](assets/MovieLens%20Recommender%20Results.png)

*Figure 14. MovieLens recommender-system results.*

---

# 6. Convolutional Neural Networks – Units 9–10

The CNN activities explored convolutional feature extraction, classification, and the limitations of image-recognition systems.

The model correctly classified a car as an automobile with **99.59% confidence**.

However, it incorrectly classified a teacup as an airplane with **52.78% confidence**.

This contrast demonstrated that confidence scores do not guarantee correctness.

It also highlighted the importance of investigating unexpected predictions and evaluating models on representative examples.

![CNN Car Prediction](assets/CNN%20Car%20and%20Teacup%20Predictions.png)

*Figure 15. CNN classification of a car.*

![CNN Teacup Prediction](assets/CNN%20Car%20and%20Teacup%20Predictions1.png)

*Figure 16. CNN misclassification of a teacup.*

The experience influenced my later medical-image project, where I placed greater emphasis on independent testing and the consequences of classification errors.

---

# 7. Unit 11 – Individual Pneumonia Detection Project

## Research Question

The individual project compared two approaches to pneumonia detection using chest X-ray images from a publicly available dataset (Mooney, 2018):

- Histogram of Oriented Gradients with a Linear Support Vector Machine.
- A custom Convolutional Neural Network.

The objective was to determine whether the more complex CNN provided a meaningful advantage over a classical machine-learning baseline. The support-vector approach is grounded in the maximum-margin classification framework described by Cortes and Vapnik (1995).

## Dataset and Evaluation

The workflow included data auditing, preprocessing, a group-aware data split, cross-validation, and an independent holdout evaluation.

The holdout contained **1,165 images**.

The project emphasised preventing data leakage and using consistent evaluation procedures.

## Model Performance

| Metric | HOG + Linear SVM | Custom CNN |
|---|---:|---:|
| Accuracy | 94.51% | 91.93% |
| Sensitivity | 95.17% | 91.17% |
| F1-score | 96.19% | 94.28% |
| False Negatives | 41 | 75 |

The HOG + Linear SVM model performed better on the independent holdout.

Its lower number of false negatives was particularly important because missed pneumonia cases may have serious clinical consequences.

![Pneumonia Performance Comparison](assets/Pneumonia%20Performance%20Comparison%20and%20Confusion%20Matrices.png)

*Figure 17. Comparison of pneumonia classification performance and confusion matrices.*

## Explainability and Grad-CAM

Grad-CAM visualisations were used to investigate image regions associated with CNN predictions, following the gradient-based localisation approach of Selvaraju et al. (2017).

Some results suggested attention to regions outside the main lung fields.

However, attention heatmaps do not prove the causal basis of a model's decision.

The activity reinforced the importance of interpreting explainability methods cautiously.

![Grad-CAM Results](assets/Grad-CAM%20Results.png)

*Figure 18. Grad-CAM visual explanations for chest X-ray classification.*

## Ethical and Professional Considerations

The project raised several important issues:

- Patient safety and false-negative predictions.
- Dataset representativeness.
- Potential shortcut learning.
- Explainability and uncertainty.
- External validation.
- Professional and clinical oversight.

The results represent an experimental comparison and do not demonstrate that either model is ready for autonomous clinical use.

---

## Evaluation of the Final Project (Unit 11) in Relation to Unit 6

No separate Unit 6 proposal for the pneumonia project was included in the available portfolio evidence. Therefore, this evaluation compares the documented Unit 6 group-project stage with the completed Unit 11 individual project rather than claiming to assess an unsubmitted proposal.

Unit 6 investigated Airbnb price prediction and supply segmentation, using regression and K-Means to address business questions. The strongest regression result was an R² of 0.623 for tuned XGBoost. Unit 11 shifted to healthcare image classification, comparing HOG–SVM with a custom CNN and placing greater emphasis on false negatives, generalisation and explainability.

On the 1,165-image holdout, HOG–SVM achieved 94.51% accuracy against 91.93% for the CNN, showing that additional complexity did not guarantee better results. Grad-CAM also exposed possible reliance on irrelevant image regions.

Together, these projects demonstrate progression from business-focused model comparison towards risk-aware evaluation. The main development was learning to judge performance against application-specific consequences, not accuracy alone.

---

# 8. Unit 11 – Model Performance Measurement

The model-performance exercise explored how changing regularisation parameters affects classification and regression results.

For logistic regression, the activity considered changes in ROC-AUC associated with different values of C.

For ridge regression, it examined the relationship between alpha and R².

This reinforced the importance of evaluating hyperparameter choices empirically and selecting metrics appropriate to the problem.

![Unit 11 Performance Results](assets/Unit%2011%20Performance%20Results.png)

*Figure 19. Unit 11 model-performance measurement results.*

---

# 9. Collaborative Discussions

## Collaborative Discussion 1 – Industry 4.0 and Industry 5.0

The first collaborative discussion explored Industry 4.0 and Industry 5.0 in healthcare, including digital transformation, interconnected systems, resilience, and human oversight.

The CrowdStrike disruption provided an example of how failures in digital infrastructure can affect essential services.

The discussion strengthened my understanding that technological efficiency must be balanced with organisational resilience and professional accountability.

![Collaborative Discussion 1 Initial](assets/Collaborative%20Discussions%201%20initial.png)

*Figure 20. Initial contribution to Collaborative Discussion 1.*

![Collaborative Discussion 1 Summary](assets/Collaborative%20Discussions%201%20summery.png)

*Figure 21. Summary reflection for Collaborative Discussion 1.*

## Collaborative Discussion 2 – AI Writers and Robo-Writers

The second collaborative discussion examined AI-assisted writing, authorship, misinformation, accountability, and professional standards.

The activity highlighted the importance of transparency and human review when generative AI is used to produce information.

I learned that the fluency of AI-generated text should not be confused with reliability or factual accuracy.

![Collaborative Discussion 2 Initial](assets/Collaborative%20Discussions%202%20initial.png)

*Figure 22. Initial contribution to Collaborative Discussion 2.*

![Collaborative Discussion 2 Summary](assets/Collaborative%20Discussions%202%20summery.png)

*Figure 23. Summary reflection for Collaborative Discussion 2.*

---

# 10. Unit 12 – Future of Machine Learning

The final unit explored emerging machine-learning approaches, including:

- Self-supervised learning.
- Neural Architecture Search.
- Edge AI.
- Ethical and sustainable AI development.

Self-supervised learning demonstrated how useful representations may be learned from unlabelled data.

Neural Architecture Search illustrated opportunities for automating model design, while raising concerns about computational requirements.

Edge AI introduced possibilities for low-latency inference and reduced dependence on cloud infrastructure.

The unit reinforced my understanding that future machine-learning systems must be evaluated for privacy, security, sustainability, and responsible deployment.

![Unit 12 Evidence](assets/Unit%2012%20Evidence.png)

*Figure 24. Unit 12 learning evidence.*

---

# 11. Reflective Case Studies

## 11.1 Model Complexity and Generalisation

### WHAT

The pneumonia project demonstrated that the classical HOG + Linear SVM approach outperformed the custom CNN on the independent holdout.

### SO WHAT

This challenged my expectation that deep learning would necessarily provide stronger performance in image classification.

I learned that greater model complexity does not automatically guarantee better generalisation.

### NOW WHAT

In future projects, I will establish transparent baseline models before introducing more complex approaches and compare them using consistent evaluation procedures.

---

## 11.2 Optimisation and Technical Risk

### WHAT

The gradient-descent experiment demonstrated that an excessively large learning rate caused the optimisation process to diverge.

### SO WHAT

This showed that seemingly small configuration decisions can produce substantial technical failures.

### NOW WHAT

I will monitor training curves, document hyperparameters, and use reproducible experiment settings.

---

## 11.3 Business Communication and Teamwork

### WHAT

The Airbnb group project received positive feedback on technical analysis but identified weaknesses in business interpretation and critical evaluation.

### SO WHAT

I recognised that technical results have limited value unless they are communicated clearly and connected to practical decisions.

### NOW WHAT

I will improve stakeholder-focused reporting, explain limitations more explicitly, and establish regular checkpoints in future virtual team projects.

---

# 12. Final Critical Reflection

This reflection follows the **WHAT, SO WHAT and NOW WHAT** framework of Rolfe, Freshwater and Jasper (2001).

## WHAT

At the beginning of the module, I mainly associated machine learning with selecting algorithms and measuring predictive accuracy.

The practical activities gradually changed this understanding.

Exploratory data analysis demonstrated the importance of identifying missing values and examining relationships before modelling.

Regression and clustering activities developed my understanding of assumptions, feature representation, and the limitations of algorithmic outputs.

The gradient-descent experiment demonstrated the importance of hyperparameter selection, while CNN exercises highlighted the difference between confidence and correctness.

The Airbnb group project and pneumonia individual project brought these lessons together in applied business and healthcare settings.

## SO WHAT

The Airbnb project showed that a model with relatively strong overall performance may still have substantial limitations in particular price categories.

Tutor feedback highlighted the importance of connecting technical findings to business value and explaining assumptions and limitations.

The pneumonia project challenged my assumptions about model complexity.

The classical HOG + Linear SVM model performed better than the custom CNN and produced fewer false negatives on the independent holdout.

This was particularly important because the consequences of classification errors depend on the application.

In healthcare, a missed positive case may be more significant than a small improvement in overall accuracy.

Grad-CAM added another dimension to my understanding of uncertainty.

Although the visualisations provided useful insights, they could not establish precisely why a prediction was made.

The collaborative discussions broadened my understanding of digital resilience, ethical responsibility, authorship, and human oversight. The initial and summary posts included in this portfolio provide evidence of engagement, although the screenshots alone do not establish the full extent of peer interaction.

Teamwork also demonstrated the importance of communication and coordination.

I recognised that task allocation should be supported by regular progress reviews, shared documentation, and collective accountability.

These experiences changed my understanding of successful machine learning.

Predictive performance remains important, but it must be interpreted alongside data limitations, explainability, practical value, and professional responsibility.

## NOW WHAT

In future machine-learning projects, I will begin with a clearer evaluation plan that includes dataset auditing, baseline models, appropriate metrics, and independent testing.

I will document preprocessing decisions, data splits, and hyperparameters to improve reproducibility.

For higher-risk applications, I will prioritise subgroup evaluation, external validation, uncertainty reporting, and human oversight.

I also intend to improve my communication of technical findings to non-technical stakeholders by connecting results to decisions and explaining limitations clearly.

In collaborative projects, I will establish regular checkpoints, clarify responsibilities early, and support structured final reviews.

The most important lesson I take from this module is that responsible machine learning requires critical judgement throughout the workflow, not simply selecting the algorithm with the highest reported score.

I will measure progress by keeping a reproducible experiment log, documenting baseline-versus-complex-model comparisons, and reviewing whether project conclusions are justified by the data. For collaborative work, I will record my own responsibilities and decisions so that individual contributions can be evidenced rather than merely described.

---

# 13. Professional Skills Matrix and Personal Development Plan

| Professional Skill | Current Evidence | Development Priority |
|---|---|---|
| Data Analysis | Auto-MPG EDA, regression, Airbnb | Improve data auditing and feature validation |
| Programming | Python, K-Means, SVM, CNN | Strengthen reproducibility and testing |
| Critical Thinking | Airbnb feedback and pneumonia comparison | Improve evaluation of limitations and uncertainty |
| Problem Solving | Gradient-descent experiments | Use systematic debugging and experiment tracking |
| Teamwork | Group project and peer evaluation | Establish regular progress checkpoints |
| Communication | Discussions and assessment reports | Explain technical findings to stakeholders |
| Ethical Awareness | CNN ethics and medical imaging | Develop fairness and external-validation skills |

## Personal Development Plan

**Short term:** Improve documentation of machine-learning experiments and strengthen evaluation procedures.

**Medium term:** Develop advanced skills in explainable AI, model calibration, and subgroup analysis.

**Long term:** Apply responsible machine-learning practices in professional projects, including transparent reporting, reproducibility, and human oversight.

---

# References

The following sources support the methodological discussion and identify the public datasets. Numerical model results are drawn from the practical and project evidence displayed above.

Breiman, L. (2001) ‘Random forests’, *Machine Learning*, 45(1), pp. 5–32. https://doi.org/10.1023/A:1010933404324

Chen, T. and Guestrin, C. (2016) ‘XGBoost: A scalable tree boosting system’, *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, pp. 785–794. https://doi.org/10.1145/2939672.2939785

Cortes, C. and Vapnik, V. (1995) ‘Support-vector networks’, *Machine Learning*, 20, pp. 273–297. https://doi.org/10.1007/BF00994018

Dgomonov (2019) *New York City Airbnb Open Data*. Kaggle. Available at: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

Mooney, P. (2018) *Chest X-Ray Images (Pneumonia)*. Kaggle. Available at: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia

Rolfe, G., Freshwater, D. and Jasper, M. (2001) *Critical Reflection in Nursing and the Helping Professions: A User's Guide*. Basingstoke: Palgrave Macmillan.

Rousseeuw, P.J. (1987) ‘Silhouettes: A graphical aid to the interpretation and validation of cluster analysis’, *Journal of Computational and Applied Mathematics*, 20, pp. 53–65. https://doi.org/10.1016/0377-0426(87)90125-7

Selvaraju, R.R. et al. (2017) ‘Grad-CAM: Visual explanations from deep networks via gradient-based localization’, *Proceedings of the IEEE International Conference on Computer Vision*, pp. 618–626. https://doi.org/10.1109/ICCV.2017.74
