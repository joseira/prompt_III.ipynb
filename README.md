# prompt_III.ipynb
# Findings:

Following initial experiments, we have further explored optimization through hyperparameter tuning and cross-validation. Our analysis reveals that the Random Forest (RF) model shows only a minimal increase in accuracy and precision after optimization. The model correctly predicts the outcome (whether someone subscribes or not) in 90% of cases.

However, the most notable outcome is that the model robustly evaluates each parameter combination and selects the optimal one, achieving a balance between performance and robustness. This ensures the model provides reliable predictions in real-world scenarios.

# Impact of some features on the model's prediction:

We found the duration of the call aligns with the earlier analysis presented in the article accompanying the dataset, which identified duration as the most influential characteristic. Specifically, longer phone calls were found to correlate with a higher likelihood of a subscription. In this context, we observe that longer phone calls remains the most relevant factor influencing the model's outcomes.

When evaluating the optimal timing for scheduling campaigns, we observe that May is the least effective month for achieving subscriptions. Additionally, specific days of the week yield better results, with Wednesday standing out as the most successful day for campaign scheduling.

# Recommendations and Conclusions

Random Forest model has demonstrated the best overall metrics in this analysis, making it a reliable tool for predicting efficiency of directed campaigns for long-term deposit subscriptions by minimizing the number of contacts required.

The model performs solidly and makes correct predictions in most cases. This is useful for providing an overview of who might be a potential subcriber and make sure they would be include in the campaing.

While the RF model is robust, it still a significant rate of false negatives, indicating that some potential subscribers are not being accurately identified. With a recall of just 54%, this leads to missed opportunities for reaching individuals who might be receptive to long-term deposit subscriptions. That's why it’s essential to focus on improving this recall metric. This will ensure that no viable prospects are overlooked, particularly those who could benefit from proactive outreach, such as being contacted by the call center.

Furthermore, key features like emp.var.rate, euribor3m, and nr.employed related with amount retained, provide valuable insights into underlying patterns that could enhance the model’s performance. By incorporating these features more effectively, the model’s predictive accuracy can be improved, which will ultimately optimize strategic planning and resource allocation. Addressing these issues will help reduce missed opportunities and ensure better-targeted marketing efforts.
