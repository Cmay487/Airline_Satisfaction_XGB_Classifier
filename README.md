## The business problem
The Airline business experiences a high proportion of neutral to dissatisfied customers and the business wants to identify areas to improve to reduce these numbers. Moreover, the business wants the capability to predict, using ML techniques, if a customer will be unhappy/neutral with the Airline when their customers leave the plane. 


## Key Methods Used 

**Bayes Theory**

1. As we are dealing with a target variable with 2 outcomes, the combination of the Binomial & Beta distributions were employed.
2. The Posterior distribution allowed the testing of how influential our Priors were -> Global Vs Noninformative Priors.
3. Analyse and quantify how reliable our proportions was by customer groups.
4. Quantify the range of expected customers to be dissatisfied by group and identify high noise features.
5. Calculate probability ranges using the Posterior distribution.
6. Bayesian Optimisation methods to fine-tune model parameters in a more "informed", cost-efficient manner.


## Key findings 

**High Baseline Dissatisfaction:** The airline currently faces a significant customer retention challenge, with 56 to 57 out of every 100 passengers disembarking with neutral or unhappy sentiments.

**Duration-Based Sensitivity:** Negative experiences compound over time. While long-haul passengers are generally more satisfied overall, the negative impacts of poor service, seating, and cleanliness are significantly magnified on longer flights, resulting in harsher brand scoring than on short-haul routes.

**The Compounding Delay Effect:** The total duration of a delay is less impactful than the combination of delays. Bayesian probability modelling demonstrates that compounded arrival and departure delays increase the probability of an unhappy customer to roughly 61%, compared to 54% for a departure delay alone—a crucial 7% difference that should directly inform operational prioritisation.

## Model performance 
**High Precision (96%):** The model correctly identifies 96 out of 100 dissatisfied customers (with only a 4% false-positive rate), providing the airline with high confidence for real-world production deployment.

**Exceptional Recall (98%):** The model successfully flags 98% of genuinely unhappy passengers, ensuring that very few dissatisfied customers slip through the net undetected.

**Production-Ready:** The outstanding overall F1 score confirms the model is highly robust and ready for immediate business use.

## Business recommendations 

1. **Proactive Service Standards:** Shift from reactive "call-bell" service to a Proactive Engagement Model. Mandate rhythmic cabin "check-ins" and transparent, frequent communication regarding operational delays to reduce passenger anxiety.
2. **Physical Comfort Mitigation:** Recognising that aircraft seating is a fixed asset, mitigate physical fatigue by providing Ergonomic Comfort Kits (lumbar cushions/enhanced blankets).
3. **Hygiene & Turnaround Audits:** Implement a mandatory Pre-Boarding Readiness Survey. Elevate cleanliness from a "task" to a "priority gate." A formal review of cleaning vendor contracts is advised to ensure deeper sanitisation across the long-haul fleet. Finally, On-Board regular cleaning activities is advised, showing customers you care about their environment cleanliness.
4. Food & Drink Offerings For any sort of delay in flight, offer free food and/or drink to the customers as a way to say sorry. I would also recommend running experiments to see the impact of such offerings to customer satisfaction.

## Future work

1. Focus on the missed features that appeared as key features in the final model.
2. Explore business value of these features.
3. If applicable, Engineer new features from the key features.

## Lessons Learned
1. Take a more holistic view of the project before dicing into the specifics.

