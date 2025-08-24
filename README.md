# Digital Twin for Wellness | Predicting Tomorrow’s Wellness from Today’s Habits
A Computer Science project involving the following research topics: Digital Twins, Machine Learning, Health Technology

### Introduction

What if we build a digital reconstruction of you? with as many data points as possible. Like a mirror of you, it is constantly updated with your data and abstracted into a single entity, which is the mirror "digital twin" of yourself. This is a cutting edge research subject at the frontier of AI, Data Science, VR/XR and simulations. It is highly multi-disciplinary and applicable across various scenarios, enabling new levels of simulations and predictions.

In this project, we will test this concept for predicting your wellness score.
### What if with the seamless data collection of today, you can know how well you're going to feel / be productive tomorrow?
Let's see.

---
### Overview & Dataset
Problem: Predict tomorrow’s wellness/productivity score (0–100) from today’s lifestyle signals.

Why it matters: Digital twins in healthcare are revolutionary, allowing for greater safety and insight into human medicine and health.

We'll use inputs commonly found from healthcare tracking gadgets nowadays.

Inputs (features): steps, exercise_mins, diet_qlt, water_l, sleep_mins, sleep_qlt, stress_avg, mood_avg, coffee_mg, prod_mins, screen_mins, rhr_avg, 

Target: wellness_tmrw (0-100)

Success: R2 >= 0.60 and RMSE <= 8 on held-out set; clear feature importance; actionable insights.

Ethics: synthetic data; no medical claims.

---

### Methods
Two models were used (both from sklearn library):

#### Linear Regression
Linear regression is the simplest hypothesis/model in AI and Machine Learning. It states:
y = mX + b

#### Random Forest
This is a much more advanced and utilized machine learning model, imported from sci-kit-learn

---

### Results

#### Scores

<img width="540" height="547" alt="linearscatter" src="https://github.com/user-attachments/assets/39a16530-4c7a-4289-a5b0-ed0e2e7ccaa4" />

##### Linear Regression R2 Score: 0.835907956827652 | Pass by standards! | Closer to 1 is better
##### Linear Regression RMSE: 7.629306511035813 | Pass by standards! | Lower is better

<img width="540" height="547" alt="rfscatter" src="https://github.com/user-attachments/assets/75edba5e-314e-4c53-9a18-9420f827ecd0" />

##### Random Forest R2 Score: 0.6182319423417859 | Pass by standards! | Closer to 1 is better
##### Random Forest RMSE: 11.637001655850122 | Fail by standards! | Lower is better

#### RF Feature importance

<img width="326" height="307" alt="featureimportance" src="https://github.com/user-attachments/assets/a9ebe419-f62a-4643-a86e-99cb8e52de6b" />

---

### Insights
* Sleep quality and time is the most important factor for tomorrow's wellness
* Linear Regression/simple models can outperform complex models when the relationship is linear.
* Stress is a critical factor, Exercise and steps (movement in general) are equally important

---

### Next Steps
* Create simple web-based dashboard to test models
* Expand dataset into real labeled data
* Collect data in real time, fulfilling digital twin application requirement, further research possible applications
* Simplify setup package, instructions, guide or framework to allow other researchers to easily implement a digital twin system

---

### Visuals

#### Correlation Heatmap
<img width="615" height="507" alt="edacorrheatmap" src="https://github.com/user-attachments/assets/bf67e5df-0d14-4830-989d-fcb4c533d3cc" />

#### Pair Plot
<img width="3190" height="3191" alt="edapairplot" src="https://github.com/user-attachments/assets/fd9881db-3538-4071-ab04-eeed0106bee3" />

---

##### Find further brief and documentation in repo! 
