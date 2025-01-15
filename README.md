Data Collection and Preparation:
Administrative information 
• 'department' – Department employees belong(ed) to 
• 'salary' – Salary level relative to rest of their department 
• 'tenure' – Number of years at the company 
• 'recently_promoted' – Was the employee promoted in the last 3 years? 
Workload information 
• 'n_projects' – Number of projects employee is staffed on 
• 'avg_monthly_hrs' – Average number of hours worked per month 
Mutual evaluation information 
• 'satisfaction' – Score for employee’s satisfaction with the company (higher is better) 
• 'last_evaluation' – Score for most recent evaluation of employee (higher is better) 
• 'filed_complaint' – Has the employee filed a formal complaint in the last 3 years?
2. Feature Engineering:
First, we have people with high 'last_evaluation' but low 'satisfaction'. Maybe these people were overqualified, frustrated, or unhappy in some other way.
Next, we have people with low 'last_evaluation' and medium 'satisfaction'. These were probably underperformers or poor cultural fits.
Finally, we have people with high 'last_evaluation' and high 'satisfaction'. Perhaps these were overachievers who found better offers elsewhere.
3. Model Selection:
Several machine learning algorithms can be used for this type of prediction, including:
Logistic Regression: A simple and interpretable model that predicts the probability of an employee leaving.
Random Forest: A powerful ensemble method that can capture complex relationships in the data.
Gradient Boosting Machines (GBM): Another ensemble method that often provides high accuracy.
The choice of model depends on the specific data and the desired balance between accuracy and interpretability.
4. Model Training and Evaluation:
Split the data: Divide the data into training and testing sets. The training set is used to train the model, while the testing set is used to evaluate its performance1 on unseen data. 
Train the model: Use the training data to train the chosen algorithm.
Evaluate the model: Use metrics such as:
Accuracy: Overall correctness of the model's predictions.
Precision: Proportion of correctly predicted leavers out of all employees predicted to leave.
Recall: Proportion of correctly predicted leavers out of all actual leavers.
AUC-ROC: Area under the Receiver Operating Characteristic curve, which measures the model's ability to distinguish between leavers and stayers.
5. Model Deployment and Monitoring:
Deploy the model: Integrate the model into your HR systems to predict the probability of current employees leaving.
Monitor the model: Regularly track the model's performance and retrain it as needed to maintain accuracy.
