
# Machine Learning – ML_PCOM7E e-Portfolio

**Student:** Essa Albuainain  
**Institution:** University of Essex Online  
**Module:** Machine Learning (ML_PCOM7E)  
**Portfolio:** https://essaalbuainain.github.io/machine-learning-eportfolio/

## Introduction and Learning Outcomes

This portfolio documents learning across Units 1–12, covering data suitability, modelling, evaluation, ethics and virtual collaboration. Evidence includes notebooks, discussions, group feedback and individual assessment. I progressed from reporting scores to questioning reliability and consequences.

## Units 1–4: Foundations, EDA and Regression

Unit 1 introduced supervised and unsupervised methods and the machine-learning lifecycle. Unit 2 Auto-MPG exploration identified six missing horsepower values and negative associations between fuel economy and vehicle weight, displacement and cylinders. Missingness and correlation required investigation before modelling.

![Auto-MPG Heatmap](assets/Auto-MPG%20Correlation%20Heatmap.jpeg)

*Figure 1. Auto-MPG correlation evidence.*

Unit 3 compared correlation, linear and polynomial regression, highlighting modelling assumptions and overfitting. Unit 4 examined fuel consumption and population–GDP relationships (2001–2021); association alone could not establish causality or predictive usefulness.

![Regression Results](assets/Correlation%20and%20Regression%20Results.jpg)

*Figure 2. Correlation and regression.*

![Population GDP](assets/Population%E2%80%93GDP%20Regression.png)

*Figure 3. Population–GDP exercise.*

## Units 5–6: Similarity and Clustering

Jaccard distances were Jack–Mary **0.7273**, Jack–Jim **0.4444**, and Jim–Mary **0.9231**; attribute representation determines similarity.

![Jaccard](assets/Jaccard%20Calculations.png)

*Figure 4. Jaccard calculations.*

The K-Means wiki examined centroid selection and cluster interpretation. Elbow plots illustrated that choosing k requires validation. Iris clustering produced **silhouette = 0.459** and **adjusted Rand index = 0.6201**. These results suggest partially meaningful clusters rather than perfect recovery of known classes (Rousseeuw, 1987).

![K-Means Wiki](assets/Wiki%20.jpeg)

*Figure 5. Wiki participation.*

![Iris Clustering](assets/Iris%20Clustering.png)

*Figure 6. Iris clustering.*

## Unit 6: Airbnb Group Project

Using New York City Airbnb data (Dgomonov, 2019), we compared Linear Regression, Random Forest (Breiman, 2001), and XGBoost (Chen and Guestrin, 2016).

| Model | Test R² |
|---|---:|
| Linear Regression | 0.501 |
| Tuned Random Forest | 0.608 |
| Untuned XGBoost | 0.617 |
| Tuned XGBoost | **0.623** |

Tuned XGBoost performed best overall, but errors varied by price band: cheaper listings were overestimated by approximately **$17**, and listings above **$500** underestimated by approximately **$866** on average. Therefore, a limited mid-market pricing pilot was more defensible than unrestricted recommendations. The group report also showed that four clusters were selected for business usefulness even though a two-cluster solution had the stronger silhouette score. That trade-off had to be disclosed rather than presented as statistical optimality.

![Airbnb Models](assets/Airbnb%20Model%20Comparison%20and%20Segmentation2.png)

*Figure 7. Model comparison.*

Four **supply-side**, not customer, clusters were identified because guest data were unavailable. The “listed but not booking” segment represented **22.5%** of listings; availability was not evidence of confirmed bookings.

![Airbnb Clusters](assets/Airbnb%20Model%20Comparison%20and%20Segmentation1.png)

*Figure 8. Supply segmentation.*

I completed my assigned section and reviewed the entire group report for coherence and presentation. The review also made me more aware of how the methods, charts and commercial conclusion must support one another rather than appear as disconnected contributions. My peer self-evaluation was **29/35**; tutor feedback encouraged stronger business interpretation and critical justification.

![Tutor Feedback](assets/Tutor%20Feedback.png)

*Figure 9. Tutor feedback.*

![Peer Evaluation](assets/Peer%20Evaluation.png)

*Figure 10. Peer evaluation.*

## Units 7–8: Neural Networks and Optimisation

Perceptron exercises explored weighted inputs, bias and AND classification. Gradient descent demonstrated parameter sensitivity: **100 iterations at 0.08** yielded cost **0.004121**, whereas **0.10** diverged to approximately **5.97 × 10²⁸**. Increasing iterations at 0.01 reduced cost from **0.480407** (100) to **0.031985** (500). MovieLens yielded **RMSE 1.0400** and **MAE 0.8358**.

![Perceptron](assets/Perceptron%20Outputs.png)

*Figure 11. Perceptron exercise.*

![Gradient 1](assets/Gradient%20Descent%20Results1.jpeg)

*Figure 12. Gradient descent.*

![Gradient 2](assets/Gradient%20Descent%20Results2.jpeg)

*Figure 13. Parameter comparison.*

![MovieLens](assets/MovieLens%20Recommender%20Results.png)

*Figure 14. Recommender performance.*

## Unit 9: CNN Classification and Ethics

Changing the test image to **`x_test[12]`** produced a correct **dog** prediction with **75.13% confidence**, verified against `y_test[12]`. This provided additional evidence beyond a single image. The true class and predicted class were checked at the same index, avoiding the misleading comparison produced when different indices were used for the image and label. Confidence remained below 100% despite correct classification.

![Unit 9 Test Image](assets/Unit9-Alternative-Test-Image.png)

*Figure 15. Alternative test image and prediction.*

The separate ethical reflection examined classification errors, dataset bias, privacy and human oversight. Responsible deployment requires robust evaluation and transparent limits (Ghallab, 2019); adversarial-image research also highlights interpretation challenges (Zhou and Firestone, 2019).

## Unit 10: CNN Feature Maps

An external car image was correctly classified at **99.59%**, while a teacup was labelled **airplane** at **52.78%**: the classifier could not reject an unfamiliar class (Hendrycks and Gimpel, 2017).

![CNN Car](assets/CNN%20Car%20and%20Teacup%20Predictions.png)

*Figure 16. Car prediction.*

![CNN Teacup](assets/CNN%20Car%20and%20Teacup%20Predictions1.png)

*Figure 17. Teacup prediction.*

Feature maps from `conv2d` revealed local pattern responses; `conv2d_1` showed more selective activations, including nearly inactive filters. ReLU permits nonlinear representation, but activation maps **do not establish the cause** of a classification.

![CNN Features 1](assets/Unit10_Intermediate_Feature_Maps_1.png)

*Figure 18. First convolutional layer.*

![CNN Features 2](assets/Unit10_Intermediate_Feature_Maps_2.png)

*Figure 19. Subsequent convolutional layer.*

## Unit 11: Individual Pneumonia Investigation

Using chest X-rays (Mooney, 2018), I compared HOG–Linear SVM (Cortes and Vapnik, 1995) with a custom CNN. Development used five group-aware folds and an independent **1,165-image holdout**. Subject grouping was inferred from filenames, not verified patient identifiers.

| Metric | HOG–SVM | CNN |
|---|---:|---:|
| Accuracy | **94.51%** | 91.93% |
| Sensitivity | **95.17%** | 91.17% |
| F1-score | **96.19%** | 94.28% |
| False negatives | **41** | 75 |

The simpler SVM outperformed the CNN. False negatives were particularly consequential, while limited demographics prevented meaningful subgroup-fairness conclusions.

![Pneumonia Results](assets/Pneumonia%20Performance%20Comparison%20and%20Confusion%20Matrices.png)

*Figure 20. Holdout results.*

Grad-CAM sometimes highlighted peripheral regions; attention visualisations suggest possible shortcuts but cannot prove model reasoning (Selvaraju et al., 2017). Neither model is clinically deployment-ready. The original dataset is limited in provenance and demographic detail; even a strong internal holdout cannot substitute for external testing across hospitals, scanners and patient populations. This was a research comparison, not a diagnostic system.

![Grad-CAM](assets/Grad-CAM%20Results.png)

*Figure 21. CNN explanations.*

**Progression from Unit 6:** Airbnb concerned price prediction and business segmentation; pneumonia required clinical sensitivity, error analysis and explainability. There was **no Unit 6 proposal for this individual project**, so this is a learning comparison, not a fabricated proposal assessment.

## Unit 11: Performance Measurement

Changing regularisation demonstrated that hyperparameter choices require empirical evidence (Pedregosa et al., 2011).

| Logistic C | ROC-AUC | Ridge α | R² |
|---:|---:|---:|---:|
| 0.001 | 0.990356 | 0 | 0.484906 |
| 0.01 | 0.995178 | 0.01 | 0.484921 |
| 0.1 | 0.997065 | 0.1 | 0.485049 |
| **1** | **0.997694** | 1 | 0.485896 |
| 10 | 0.994549 | 10 | 0.488092 |
| 100 | 0.983648 | **100** | **0.490477** |

The highest tested AUC occurred at **C = 1**; the highest tested R² at **α = 100**. Neither establishes a universal optimum.

![Unit 11 Regularisation](assets/Unit%2011%20Performance%20Results.png)

*Figure 22. Performance measurement.*

## Collaborative Discussions

Discussion 1 addressed Industry 4.0/5.0, healthcare resilience and responsible human oversight during widespread digital disruption.

![Discussion 1 Initial](assets/Collaborative%20Discussions%201%20initial.png)

*Figure 23. Initial contribution.*

![Discussion 1 Summary](assets/Collaborative%20Discussions%201%20summery.png)

*Figure 24. Summary.*

![Discussion 1 Reply A](assets/Discussion1-Peer-Reply.jpeg)

*Figure 25. Peer reply one.*

![Discussion 1 Reply B](assets/Discussion1-Peer-Reply2.jpeg)

*Figure 26. Peer reply two.*

Discussion 2 considered AI writing, authorship, verification and accountability: generative AI may raise writing productivity (Noy and Zhang, 2023) while narrowing collective creative diversity (Doshi and Hauser, 2024).

![Discussion 2 Initial](assets/Collaborative%20Discussions%202%20initial.png)

*Figure 27. Initial contribution.*

![Discussion 2 Summary](assets/Collaborative%20Discussions%202%20summery.png)

*Figure 28. Summary.*

![Discussion 2 Reply A](assets/Discussion2-Peer-Reply.jpeg)

*Figure 29. Peer reply one.*

![Discussion 2 Reply B](assets/Discussion2-Peer-Reply2.jpeg)

*Figure 30. Peer reply two.*

## Unit 12 and Professional Development

Unit 12 examined self-supervised learning, Neural Architecture Search, Edge AI and sustainability. These methods raise important computational, privacy and environmental trade-offs requiring careful governance. I intend to strengthen reproducibility, external validation, stakeholder communication and ethical assessment.

![Unit 12](assets/Unit%2012%20Evidence.png)

*Figure 31. Future-learning activity.*

---

# Final Critical Reflection

This reflection uses the **What? So What? Now What?** model (Rolfe, Freshwater and Jasper, 2001).

## WHAT? Learning Experiences

At the beginning of this module, I thought successful machine learning mainly involved choosing an algorithm and reporting the highest accuracy. Across twelve units, I discovered that data suitability, reproducibility, assumptions, error analysis, communication and ethical consequences are equally important. Practical exercises challenged me to connect abstract concepts with observable behaviour rather than accept results without questioning them.

In earlier exercises, I tended to regard a completed notebook and a plausible figure as evidence of success. By later units, I was checking whether splits were defensible, whether metrics matched the intended use and whether an explanation supported the conclusion.

The Auto-MPG activity showed why missing values and correlated features require investigation before modelling. The Jaccard exercise demonstrated that similarity depends on selected categorical attributes. Iris clustering revealed the difference between discovering groups and reproducing known labels: its silhouette and adjusted Rand results indicated meaningful but imperfect separation. These exercises encouraged me to examine the data before interpreting scores.

Gradient descent made optimisation tangible. Changing the learning rate from 0.08 to 0.10 caused dramatic divergence, demonstrating that parameter selection determines whether learning succeeds. The CNN activities challenged my interpretation of confidence. An alternative image was correctly recognised as a dog, while the external teacup received an incorrect label. Feature maps revealed internal activity without conclusively explaining the prediction.

Two assessments posed distinct challenges: the Airbnb group project applied regression and clustering to a business problem, while my individual pneumonia investigation compared medical-image classifiers. Both required matching evaluation criteria to decisions rather than using generic performance measures.

## SO WHAT? Critical Evaluation

The Airbnb project demonstrated the limits of aggregate metrics. Tuned XGBoost achieved the strongest overall R², but errors varied across prices. Expensive properties were systematically underestimated, while cheaper listings were overestimated. A model appearing satisfactory overall could therefore mislead particular groups of hosts. I learned that error analysis by price band and clear deployment boundaries matter alongside headline performance.

Tutor feedback requested stronger business interpretation and justified recommendations, challenging my focus on technical competence. I completed my assigned section and reviewed the full report for coherence and presentation. Reading it revealed how easily individually written sections can become disconnected. My peer self-evaluation of 29/35 reflected participation but also opportunities for better coordination. In future, I will agree expectations earlier, schedule review checkpoints and ensure recommendations follow the evidence.

This feedback also made me reconsider my contribution. Reviewing a finished report is useful, but intervening sooner would have allowed problems in scope, interpretation or consistency to be corrected before they reached the final draft. I therefore see teamwork as an iterative analytical responsibility, not merely combining completed sections.

The pneumonia project challenged my assumption that deep learning would outperform classical approaches. HOG–SVM achieved higher accuracy and sensitivity than the CNN despite its simpler design. False negatives were especially important: 41 for SVM versus 75 for CNN. In healthcare, missing pneumonia may delay investigation. I learned to prioritise application-specific error consequences instead of relying solely on accuracy.

I became cautious about rigorous evaluation. The project used a holdout and filename-inferred subject grouping to limit leakage, but these identifiers were not confirmed patient records. Reliable demographic information was unavailable for meaningful fairness assessment. Consequently, holdout performance does not establish clinical generalisability or equity. Reporting these limitations openly is preferable to concealing them behind favourable results.

Grad-CAM complicated my interpretation of CNN predictions. Some activations appeared outside lung fields, suggesting possible shortcut learning. Yet an attention map cannot establish causality. I now regard explanations as supporting evidence requiring testing, not definitive proof of appropriate model reasoning (Selvaraju et al., 2017).

Collaborative discussions extended these lessons beyond modelling. Industry 4.0/5.0 raised concerns about resilience and oversight when essential services rely on digital systems. The AI-writing debate revealed tensions between productivity, originality and responsibility. Research suggests individual writing benefits but possible reductions in collective diversity (Noy and Zhang, 2023; Doshi and Hauser, 2024). Professional responsibility includes checking outputs, disclosing limitations and retaining accountability.

## NOW WHAT? Development Actions

My immediate goal is reproducible experimentation. I will document dataset provenance, cleaning, data partitions, random seeds, baselines and hyperparameters. I will reserve independent evaluation data wherever feasible rather than repeatedly tune against a final test set. The regularisation exercise reinforced why parameter choices require evidence.

To measure improvement, I will maintain an experiment log for my next project and review it before reporting results. I will specify success criteria in advance, include at least one baseline and document outcomes. These actions should make reports more auditable.

Second, I will evaluate models beyond aggregate scores. For regression, I will investigate price-band errors and communicate uncertainty. For higher-risk classification, I will examine sensitivity, false negatives, calibration and available subgroups. Missing demographic or external-validation evidence must be acknowledged rather than treated as evidence of readiness.

Third, I will improve teamwork by agreeing responsibilities, scheduling intermediate reviews and checking consistency across sections. I will communicate results more clearly to non-technical stakeholders, linking recommendations to evidence, uncertainty and limitations.

In the medium term, I will strengthen experiment tracking, explainability and external validation. Longer term, I hope to apply machine learning where decisions can be scrutinised. My central lesson is that a successful model is not necessarily the highest-scoring one. Success also requires sound data, transparent evaluation, safeguards and recognition of what evidence cannot establish.

---

# References

Breiman, L. (2001) ‘Random forests’, *Machine Learning*, 45(1), pp. 5–32. https://doi.org/10.1023/A:1010933404324

Chen, T. and Guestrin, C. (2016) ‘XGBoost: A scalable tree boosting system’, *Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining*, pp. 785–794. https://doi.org/10.1145/2939672.2939785

Cortes, C. and Vapnik, V. (1995) ‘Support-vector networks’, *Machine Learning*, 20, pp. 273–297. https://doi.org/10.1007/BF00994018

Dgomonov (2019) *New York City Airbnb Open Data*. Kaggle. Available at: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data (Accessed: 14 October 2026).

Doshi, A.R. and Hauser, O.P. (2024) ‘Generative AI enhances individual creativity but reduces the collective diversity of novel content’, *Science Advances*, 10(28), eadn5290. https://doi.org/10.1126/sciadv.adn5290

Ghallab, M. (2019) ‘Responsible AI: requirements and challenges’, *AI Perspectives*, 1, article 3. https://doi.org/10.1186/s42467-019-0003-z

Hendrycks, D. and Gimpel, K. (2017) ‘A baseline for detecting misclassified and out-of-distribution examples in neural networks’, *International Conference on Learning Representations*. Available at: https://arxiv.org/abs/1610.02136 (Accessed: 14 October 2026).

Mooney, P. (2018) *Chest X-Ray Images (Pneumonia)*. Kaggle. Available at: https://www.kaggle.com/datasets/paultimothymooney/chest-xray-pneumonia (Accessed: 14 October 2026).

Noy, S. and Zhang, W. (2023) ‘Experimental evidence on the productivity effects of generative artificial intelligence’, *Science*, 381(6654), pp. 187–192. https://doi.org/10.1126/science.adh2586

Pedregosa, F. et al. (2011) ‘Scikit-learn: Machine learning in Python’, *Journal of Machine Learning Research*, 12, pp. 2825–2830. Available at: https://jmlr.org/papers/v12/pedregosa11a.html (Accessed: 14 October 2026).

Rolfe, G., Freshwater, D. and Jasper, M. (2001) *Critical Reflection in Nursing and the Helping Professions: A User's Guide*. Basingstoke: Palgrave Macmillan.

Rousseeuw, P.J. (1987) ‘Silhouettes: A graphical aid to the interpretation and validation of cluster analysis’, *Journal of Computational and Applied Mathematics*, 20, pp. 53–65. https://doi.org/10.1016/0377-0426(87)90125-7

Selvaraju, R.R. et al. (2017) ‘Grad-CAM: Visual explanations from deep networks via gradient-based localization’, *Proceedings of the IEEE International Conference on Computer Vision*, pp. 618–626. https://doi.org/10.1109/ICCV.2017.74

Zhou, Z. and Firestone, C. (2019) ‘Humans can decipher adversarial images’, *Nature Communications*, 10, article 1334. https://doi.org/10.1038/s41467-019-08931-6
