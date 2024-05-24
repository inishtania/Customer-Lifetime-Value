# ⭐ Capstone 03: Customer Lifetime Value<br />
One study indicates that the order value from existing customers is 31% higher than that from first-time buyers. It is also a fact that selling to existing customers who are satisfied with our service is much easier than attracting new customers. There's also a general rule of thumb that acquiring new customers costs nearly 5 times more than retaining existing ones.

As a result, over time, a fundamental business metric known as Customer Lifetime Value (CLV) has been developed. This metric helps companies evaluate the potential of their customers and even map out future prospects.

CLV is calculated by counting the total transactions a customer makes over a period of time. The longer the period (or customer lifespan) and the higher the number of transactions, the greater the CLV.

## **Goals of This Project**
As a data scientist, I was asked by the customer relationship division to create a tool to predict customer lifetime value for the future.
By having this tool, the company will be able to create strategies for retaining customers and ensuring they are satisfied with the company's service.

## **Approach and method**
Utilizing historical data and various features, we will find the best regression model that fits the data and enables the company to predict future CLV also identify the most important features.
<br>

## **Evaluation Method**
The evaluation metrics to be used are RMSE, MAE, and MAPE. RMSE is the root mean square error, MAE is the mean absolute error, and MAPE is the mean absolute percentage error produced by the regression model. The smaller the values of RMSE, MAE, and MAPE, the more accurate the model is in predicting clv based on the features used.

## **The Result**
After conducting 4 experiments, the best model identified is the `Random Forest without any hyperparameter tuning` and then it needed to `delete outlier` where we delete the customer that has more than 8 policy and has been claim more than $2.000 

This model performs well in evaluating Customer Lifetime Value (CLV) within the range of $9,000 to $10,000, which corresponds to the third quartile (Q3) of the CLV distribution. Therefore, this data effectively represents:

- Customers with 1 to 4 insurance policies.
- Customers with a monthly auto premium of $61 to $109.
- Customers with a total claim amount up to $550.
- Customers with an income range of $0 to $62,500.

The model achieved a Mean Absolute Percentage Error (MAPE) of 10.89%, indicating that the model's predictions could deviate by up to 10.89% from the actual values, particularly for customers within the specified ranges. However, the model might exhibit higher error rates due to potential bias.

Analyzing feature importance from the model reveals that the most significant features are the `number of policies`, `monthly auto premium`, `total claim amount` , `income and education`. This makes sense because CLV calculations are primarily based on the number of transactions made by customers

Combining this with the SHAP values, the `vehicle class`, especially for those who own `sports cars`, can make clv more varied. 

## **Linkedin**
Pleaase kindly check my profile because i kept update my work on linkedin www.linkedin.com/in/intania-iskandar-35b526285
