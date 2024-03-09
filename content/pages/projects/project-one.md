---
type: ProjectLayout
title: Human or Robots?
colors: colors-a
date: '2021-12-31'
client: Facebook
description: >-
  Human bidders on the site are becoming increasingly frustrated with their inability to win auctions vs. their software-controlled counterparts. As a result, usage from the site's core customer base is plummeting.
featuredImage:
  type: ImageBlock
  url: /images/bgrobot.jpg
  altText: Project thumbnail image
media:
  type: ImageBlock
  url: /images/bgrobot.jpg
  altText: Project image
---

Embark on a machine learning journey with the Facebook and Kaggle Engineering competition (2015) aimed at eliminating unfair auction activity. In this project, my task was to develop a model that identifies bids placed by "robots" on an online auction site, addressing the frustration of human bidders and stemming the decline in user engagement.


Problem Definition: Understand the challenges faced by the online auction site, where human bidders are losing auctions to their software-controlled counterparts, leading to a decline in site usage.

Tasks 1 - Data Analysis.

Dive into the provided data from the online platform, examining bid behavior, frequency, and patterns to comprehend the dynamics of robot-generated bidding.

Task 2 - Model Development.

Utilize machine learning techniques to create a robust model capable of identifying bids placed by robots. Leverage behavioral data, including bid frequency over short periods, to enhance the model's accuracy.

Task 3 - Evaluation.

Assess the model's effectiveness in flagging users exhibiting robot-like bidding behavior. Fine-tune the model to achieve optimal performance.

Task 4 - Customer Happiness Restoration.

Contribute to rebuilding customer happiness by providing the site owners with an effective solution to eliminate computer-generated bidding from their auctions.

> “Completed the project with a private AUC score of 0.935 and a public AUC score of 0.8941 ”

Learning Pointers

Through this project Ive learnt the importance of feature engineering, being able to critically identify differences in bidding behaviour to differentiate bots and humans then harness the difference and further highlight them.

Ultimately after building over 30 features I have found the following features to be the most effective
1. Bids per auction
2. Device per bid
3. bid_id
4. device_per_auction_bid
5. ip_per_bid
6. mean_bot_per_country
7. response_time

Through the use of Gradient boosting classfier I managed to achieve a high AUC (Area Under the ROC Curve) results for several reasons:

Ensemble Method
Gradient Boosting is an ensemble learning technique that combines the predictions of multiple weak learners (typically decision trees) to create a strong predictive model.
By sequentially adding weak learners and adjusting weights based on errors, it can improve the model's overall performance.

Robustness to Overfitting
Gradient Boosting tends to be less prone to overfitting compared to individual decision trees, as it iteratively corrects errors in the training process.

Handling Nonlinear Relationships
Gradient Boosting can capture complex, nonlinear relationships in the data, making it effective in scenarios where simple linear models may fall short.

Feature Importance
It provides insights into feature importance, helping you identify which features contribute most to the model's performance. This is valuable for understanding the underlying patterns in the data.
Probability Estimation:

Gradient Boosting classifiers provide probability estimates for predictions, which is crucial for computing AUC. The predict_proba method in sklearn returns the probability estimates, allowing the calculation of AUC.

Fine-Tuning Parameters
Gradient Boosting offers parameters like learning rate, tree depth, and the number of trees that can be fine-tuned to optimize performance.

Visit my github to find out more!
