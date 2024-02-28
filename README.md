# Verizon Customer Default Prediction Model

## Background
Verizon Communications, facing risks in their phone contract business, needs to identify customers likely to default on payments. Providing phones as part of service agreements poses a financial risk akin to lending. Our goal is to develop an application for in-store use that aids staff in deciding on customer contract approvals.

## Business Problem
Verizon faces a challenge with customers defaulting on their contracts after receiving high-value phones(worth >$1000). The task is to develop a predictive model that can be used in real-time to evaluate the risk of default and inform the decision on whether to approve a phone contract.
**The objective is to build a predictive model for in-store use, aiding the approval or rejection of customer applications.**

<img width="273" alt="image" src="https://github.com/ColleenJung/Verizon-Case/assets/119357849/5d2ea056-5a69-41c8-9eeb-371552faa047">

## Our Solution
Our team developed a predictive model to assess the risk of customer default. We chose a model that balances the risk of loss from defaults with the opportunity cost of false rejections, aiming to enhance Verizon's profit retention.

## Methodology Selection
### [Confusion matrix](https://medium.com/analytics-vidhya/confusion-matrix-accuracy-precision-recall-f1-score-ade299cf63cd)
<img width="421" alt="Screenshot 2024-02-27 at 10 27 46 PM" src="https://github.com/ColleenJung/Verizon-Case/assets/119357849/6a3f9981-c8ed-48c1-b8fb-efadea210036">

**1. Accuracy:**
- represents the number of correctly classified data instances over the total number of data instances.

![image](https://github.com/ColleenJung/Verizon-Case/assets/119357849/756ddfef-aa3c-4eb0-990b-870f1efdf27e)

- Is accuracy the best measure?
Accuracy may not be a good measure if the dataset is not balanced (both negative and positive classes have different number of data instances). 

**2. Precision:**
- Precision should ideally be 1 (high) for a good classifier.
- Precision becomes 1 only when the numerator and denominator are equal i.e TP = TP +FP, this also means FP is zero. 

![image](https://github.com/ColleenJung/Verizon-Case/assets/119357849/0b301b88-2d14-44ae-ad3c-45e6e34a9ed1)

**3. Recall:**
- known as sensitivity or true positive rate and is defined as follows
- Recall should ideally be 1 (high) for a good classifier. Recall becomes 1 only when the numerator and denominator are equal i.e TP = TP +FN, this also means FN is zero. 
![image](https://github.com/ColleenJung/Verizon-Case/assets/119357849/6b00c7a2-b19c-49ef-ac5e-91ea41081f3e)

**4. F1 Score:**
- F1-score is a metric which takes into account both precision and recall and is defined as follows:
- F1 Score becomes 1 only when precision and recall are both 1. F1 score becomes high only when both precision and recall are high. F1 score is the harmonic mean of precision and recall and is a better measure than accuracy.
![image](https://github.com/ColleenJung/Verizon-Case/assets/119357849/5d9e93be-025d-47cd-9e6c-c8fb8b5c39ce)

**(To summarise the differences between the F1-score and the accuracy)[https://medium.com/analytics-vidhya/accuracy-vs-f1-score-6258237beca2]**

- **Accuracy** is used when the True Positives and True negatives are more important while **F1-score** is used when the False Negatives and False Positives are crucial
- **Accuracy** can be used when the class distribution is similar while **F1-score** is a better metric when there are imbalanced classes as in the above case.
- In most real-life classification problems, **imbalanced** class distribution exists and **thus F1-score is a better metric to evaluate our model on.**


## Model Performance
The model's effectiveness was gauged not only by traditional statistical measures but also by its financial impact. We estimated the model's value by the potential dollar change per million applicants.

<img width="488" alt="image" src="https://github.com/ColleenJung/Verizon-Case/assets/119357849/2b64fa36-b098-45a3-be45-fa8d35aa7db5">


## Business Value
Assuming one million applicants, an 80% current approval rate, and an 11.5% default rate among approved applicants, our model aims to reduce defaults significantly. We projected the financial impact considering both direct losses from defaults and potential profits from long-term customer retention.

### Assumptions and Estimates
- Current default rate of approved applicants: 11.5%
- Loss per default: Approx. $1000
- Profit per paying customer over 36 months: Approx. $250
- Assumed default rate for rejected applicants: Less than 50%

Our model provides a credible estimate of the business value, with assumptions clearly outlined for transparency.

