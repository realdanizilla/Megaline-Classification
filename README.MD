# Megaline Plan Transition Recommendation

## Table of Contents
- [Megaline Plan Transition Recommendation](#megaline-plan-transition-recommendation)
  - [Table of Contents](#table-of-contents)
  - [Project Objective](#project-objective)
  - [Project Structure and Steps](#project-structure-and-steps)
  - [Tools and Techniques Utilized](#tools-and-techniques-utilized)
  - [Specific Results and Outcomes](#specific-results-and-outcomes)
  - [What I Have Learned from This Project](#what-i-have-learned-from-this-project)

## Project Objective

The goal of this project is to develop a classification model for the cellular provider Megaline, which aims to analyze customer behavior and recommend one of the two new plans: Smart or Ultra. Megaline wants to encourage its customers to transition to these newer plans and improve customer satisfaction while optimizing its revenue streams.

[back to top](#megaline-plan-transition-recommendation)

## Project Structure and Steps

**1. Data Loading and Preparation:**

- The dataset (users_behavior.csv) contains monthly behavioral information about users, including the number of calls, call duration in minutes, number of messages, and internet traffic usage in MB. The plan currently used by the customer is also indicated (is_ultra column).
- Data was examined for types, missing values, and potential optimizations, such as converting floating-point columns for calls and messages to integers.
- The data was split into three sets: training, validation, and testing, ensuring balanced and reproducible splits.

**2. Model Selection and Training:**

- Since the problem is a binary classification between the two plans (Smart and Ultra), multiple models were considered: Decision Tree Classifier, Random Forest Classifier, and Logistic Regression.
- Each model was trained using different hyperparameters to optimize for accuracy.

**3. Model Optimization and Evaluation:**

- A Grid Search was implemented to optimize hyperparameters for each model.
- The performance of each model was evaluated using accuracy as the primary metric.
- The final model's accuracy was validated using the test dataset to ensure it met the required threshold of 0.75.

**4. Results Analysis and Validation:**

- Each model's best-performing hyperparameters were identified, and their accuracy scores were recorded.
- A conclusive model was selected based on its performance on unseen test data, achieving optimal accuracy.

[back to top](#megaline-plan-transition-recommendation)

## Tools and Techniques Utilized

**Libraries:**
- pandas, numpy: For data manipulation and preparation.
- scikit-learn: For model training, optimization, and evaluation.

**Models and Methods:**
- Decision Tree Classifier: To explore simple tree-based rules for classifying user behavior into Smart or Ultra plans.
- Random Forest Classifier: For ensemble learning to improve model accuracy and robustness.
- Logistic Regression: As a baseline model to determine the relationship between the input features and the binary target variable.
- Grid Search: To tune model hyperparameters for optimal performance.

**Model Evaluation:**

- Accuracy score for evaluating model performance on validation and test datasets.

[back to top](#megaline-plan-transition-recommendation)

## Specific Results and Outcomes

- The **Decision Tree Model** achieved a maximum accuracy of approximately 78.5% on the validation set with a depth of 3.
- The **Random Forest Model** provided better results with a tuned accuracy of around 81.9% on the validation set using the best parameters.
- The **Logistic Regression Model** encountered convergence issues but was successfully tuned for accuracy.
- The final model selection achieved an accuracy exceeding the 0.75 threshold, validating the model's effectiveness in classifying customers into the Smart or Ultra plans accurately.

[back to top](#megaline-plan-transition-recommendation)

## What I Have Learned from This Project

- **Data Preprocessing and Handling**: Learned to clean and prepare large datasets, ensuring appropriate data types and handling missing values effectively.
- **Model Selection and Hyperparameter Tuning**: Gained experience in selecting appropriate machine learning models and tuning their parameters to achieve the best accuracy.
- **Model Evaluation**: Developed the ability to evaluate and validate models using metrics like accuracy and understand their trade-offs.
- **Technical Proficiency**: Improved proficiency with pandas, scikit-learn, and model selection techniques, allowing for a deeper understanding of the behavior of different classification algorithms.

[back to top](#megaline-plan-transition-recommendation)