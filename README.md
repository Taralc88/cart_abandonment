# MyCoke360 Cart Abandonment Analysis

## Project Summary
Swire Coca-Cola’s MyCoke360 platform supports business-to-business orders, but a significant share of sessions end with items left in the cart and no order submitted. These incomplete orders represent lost revenue and signal friction within the digital ordering experience.  

This project focuses on understanding why customers get stuck, identifying behavioral patterns tied to abandonment, and providing data-driven recommendations to improve the ordering process.

---

## Business Problem & Objective
The goal is to identify behaviors associated with incomplete purchases and determine where users encounter friction. By analyzing session-level activity, we aim to reveal the patterns that separate finished orders from those that stop early, enabling the business to reduce cart abandonment and increase order revenue.

---

## Group Solution Overview
Our team built a multi-step analytical workflow:

1. **Feature Engineering**

   We created session-level variables representing engagement, cart interactions, and timing behaviors.

   **Key features included:**
   - `purchase_to_cart_ratio` (strongest predictor)
   - add/remove/update cart patterns
   - session duration and timing
   - quick vs. long session indicators

2. **Modeling**

   We trained classification models to understand which behaviors most strongly predict whether an order is finished or abandoned.  
   The purchase-to-cart ratio, cart activity, and session depth emerged as top signals.

3. **Behavioral Clustering**

   We performed k-means clustering to segment sessions into four behavioral groups:
   - **High-intent, high-friction users** who engage heavily but still abandon  
   - **Moderate-intent browsers**  
   - **Quick, low-intent weekday lookups**  
   - **Quick evening drop-ins**

4. **Recommendations**

   The analysis identified a specific high-intent segment (Cluster 3) that engages heavily but still struggles in checkout. We recommended several changes to reduce friction and improve order completion:

   - Streamline the checkout flow  
   - Surface fees earlier in the process  
   - Reduce required steps or clicks  
   - Simplify cart editing  
   - Improve error messaging and feedback 

---

## My Individual Contribution
I focused on:

- Building and validating the session-level feature engineering  
- Creating the behavioral clustering pipeline and interpreting cluster meaning  
- Integrating the `purchase_to_cart_ratio` metric into clustering  
- Designing heatmaps and visual diagnostics for cluster behavior  
- Drafting the behavioral insights section for the presentation  
- Helping tie model features to behavioral segments for business storytelling  
- Cleaning and debugging the k-means code to ensure stable, interpretable clusters  

---

## Challenges We Encountered

- Handling large amounts of missing or sparse behavioral data  
- Cleaning session-level events so they aligned with purchase outcomes  
- Avoiding noisy features that disrupted clustering  
- Explaining behavioral clusters in a way non-technical stakeholders can understand  
- Integrating modeling results with behavioral patterns in a cohesive story  

---

## What I Learned
This project strengthened my skills in:

- Translating messy behavioral logs into structured features  
- Using k-means clustering for behavioral segmentation  
- Connecting model outputs to real customer behavior  
- Evaluating meaningful engagement vs. noise  
- Communicating technical findings as business insights  

It also reinforced how important it is to look beyond model accuracy and understand the behavior behind the predictions.

