# Recidivism Case Study

This case study is based on two articles that were published in 2016:

* "[Machine Bias](https://www.propublica.org/article/machine-bias-risk-assessments-in-criminal-sentencing)", by Julia Angwin, Jeff Larson, Surya Mattu and Lauren Kirchner, and published by [ProPublica](https://www.propublica.org).

* A response by Sam Corbett-Davies, Emma Pierson, Avi Feller and Sharad Goel: "[A computer program used for bail and sentencing decisions was labeled biased against blacks. It’s actually not that clear.](https://www.washingtonpost.com/news/monkey-cage/wp/2016/10/17/can-an-algorithm-be-racist-our-analysis-is-more-cautious-than-propublicas/)", published in the Washington Post.

Both articles are about [COMPAS](https://en.wikipedia.org/wiki/COMPAS_(software)), a statistical tool used in the justice system to assign defendants a "risk score" that is intended to reflect the risk that they will commit another crime if released.

The ProPublica article evaluates COMPAS as a binary classifier, and compares its error rates for black and white defendants.  It concludes that COMPAS is unfair to black defendants because they are more likely to be misclassified as high risk.

In response, the Washington Post article shows that COMPAS has the same predictive value black and white defendants.  And they explain that the test cannot have the same predictive value and the same error rates at the same time.

The purpose of this case study is to understand these conflicting claims, to learn about classification algorithms and the metrics we use to evaluate them, and to think about fairness and the ethics of algorithms.

* [In the first notebook](https://colab.research.google.com/github/AllenDowney/RecidivismCaseStudy/blob/master/01_classification.ipynb) I replicate the analysis from the ProPublica article and define the basic metrics we use to evaluate classification algorithms, including error rates and predictive values.

* [In the second notebook](https://colab.research.google.com/github/AllenDowney/RecidivismCaseStudy/blob/master/02_calibration.ipynb) I replicate the analysis from the WaPo article and define the calibration curve, the ROC curve, and a related metric, concordance. 

* [In the third notebook](https://colab.research.google.com/github/AllenDowney/RecidivismCaseStudy/blob/master/03_fairness.ipynb) I use the same methods to evaluate the performance of COMPAS for male and female defendants, and lay out the fundamental conflict between two definitions of fairness.



