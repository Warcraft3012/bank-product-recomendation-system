# bank-product-recomendation-system
1. Overview:

This project aims to build a series of recommendation systems to provide customized product offerings to the customers in Product Recommendation challenge. As a Data Scientist it is an excellent learning opportunitiy to gain the knowledge of how to establish a recommendation system from 0 - 1 and use the real life case to get hands dirty. Given there are many fantastic algorithms in the recommendation system field, this project is using 3 traditional yet powerful techniques:

1) Memory-based Collaborative Filtering: User-based and Item-Based Models

2) Model-based Collaborative Filtering: Matrix Factorization (Funk SVD)

3) ML: GBDT + LR (Gradient Boosting Decision Tree + Logistic Regression)

And for the Cold Start phase where new customer are just opened their account but no transaction or product purchase history, this project will use the Popularity-based Mode to recommendation the most hot saling product to them.

The project will also evaluate the performance across all these models and discuss some use cases, risks and production procedures of the recommendation system in reality.
2. Project Steps:

1) Data Import and Profiling: import all the required data and take a quick check on its quality;

2) Data Cleaning: inpute missing values, drop unused fields and anything else to enhance the data integraty;

3) Feature Engineering: transform the original features into new versions for the training task;

4) Model Training: build and train the models listed above using the data prepared in the last step;

5) Recommendation: recommend the products to the customers based on their purchasing history and features. Also test the model's performance using test split.

6) Implement & Improvement: how the model can be utilized in the real life cases, potential risks and improvement ideas.
Implement & Improvement:
1. Implementation
When the recommendation model is built and originally tested using the validation data, it would be nessary to use the following period's real examples to thoroughly evaluate its performance using appropriate evaluation metrics and validation techniques. This step helps you verify that the model is accurate and reliable.

Then, it is important to align the model with the current infrasturture of the bank (e.g. CRM, Mobile APP, Website Account) so that the API could be utilized to transload the recommendation data to the user. Also it would be important to implement A/B testing to evaluate the effectiveness of your recommendation model compared to alternative approaches. This helps in refining and optimizing the model over time based on user feedback and business goals.

At the same time, since banking industry is highly regularized, the system should comply with all relevant privacy regulations and safeguards customer data appropriately before it is put into use.

2. Improvement
The project is a simplified version of the real-life product recommendation in the banking industry. There are a few improvement ideas for the future work:

Feature Selection and Engineering: given only the customer features and purchasing behaviour available in this project, it would be much helpful to include more product features (such as their category, customer setment, term, risk level, profitability and variance) into the recommendation model to generate more accurate and realizable recommendations.

Training and testing dataset: in the real-life use cases, more periodic training data should be used to train the model since more data would provide more holistic view of the population characteriastic. Besides, the advanced infrasturture (e.g. Cloud Storage and Computation) should be utilized to enhance the model training process.

Recommendation Methods: although the models used in the project are classic and effective in the industry, there are more advanced deep learning models such as YouTubeDNN, DeepFM that could learn more complex patterns from the training data and generate more accurate recommendations. Besides, hybird model (a model combines more than one recommendation algorithms) can be used to enhance the prediction power as well.
