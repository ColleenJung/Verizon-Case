# Verizon Customer Default Prediction Model

## Background
Verizon Communications, facing risks in their phone contract business, needs to identify customers likely to default on payments. Providing phones as part of service agreements poses a financial risk akin to lending. Our goal is to develop an application for in-store use that aids staff in deciding on customer contract approvals.

## Business Problem
Verizon faces a challenge with customers defaulting on their contracts after receiving high-value phones(worth >$1000). The task is to develop a predictive model that can be used in real-time to evaluate the risk of default and inform the decision on whether to approve a phone contract.
*Promt1- Verizon’s end goal is an application that can be used by Verizon staff within a store to approve or reject an application during live customer interactions.

## Our Solution
Our team developed a predictive model to assess the risk of customer default. We chose a model that balances the risk of loss from defaults with the opportunity cost of false rejections, aiming to enhance Verizon's profit retention.

## Model Performance
The model's effectiveness was gauged not only by traditional statistical measures but also by its financial impact. We estimated the model's value by the potential dollar change per million applicants.

## Business Value
Assuming one million applicants, an 80% current approval rate, and an 11.5% default rate among approved applicants, our model aims to reduce defaults significantly. We projected the financial impact considering both direct losses from defaults and potential profits from long-term customer retention.

### Assumptions and Estimates
- Current default rate of approved applicants: 11.5%
- Loss per default: Approx. $1000
- Profit per paying customer over 36 months: Approx. $250
- Assumed default rate for rejected applicants: Less than 50%

Our model provides a credible estimate of the business value, with assumptions clearly outlined for transparency.

