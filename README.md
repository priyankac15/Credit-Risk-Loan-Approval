# CreditRisk: Loan-Approval Model
The project objective is to develop a predictive model that can accurately classify loan applicants as good or bad credit risks. The model should assist the bank executives in making loan approval decisions and reduce the risk of default.

<h1> The scope of the project includes the following: </h1>

- <b> Data collection and pre-processing:</b> This involves obtaining the dataset, cleaning and formatting the data, and preparing it for analysis.

- <b> Exploratory data analysis:</b> This involves understanding the data through visualization and statistical analysis.

- <b> Feature selection:</b> This involves selecting the most relevant features to be included in the predictive model.

- <b> Model development:</b> This involves building, training, and testing several machine learning models to predict credit risk.

- <b> Model evaluation and selection:</b> This involves evaluating the performance of the models and selecting the best model for deployment.

<b> The goal of the project is to develop a predictive model that can accurately classify loan applicants as good or bad credit risks with a high degree of accuracy. This will reduce the risk of default and improve the bank's profitability.</b>

<h2> Data description </h2>

The business meaning of each column in the data is as below:

- GoodCredit: Whether the issued loan was a good decision or bad.
- checkingstatus: Status of existing checking account.
- duration: Duration of loan in months.
- history: Credit history of the applicant.
- purpose: Purpose for the loan
- amount: Credit amount
- savings: Savings account/bonds
- employ: Present employment since
- installment: Installment rate in percentage of disposable income
- status: Personal status and sex
- others: Other debtors / guarantors for the applicant
- residence: Present residence since
- property: Property type of applicant
- age: Age in years
- otherplans: Other installment plans
- housing: Housing
- cards: Number of existing credits at this bank
- job: Job
- liable: Number of people being liable to provide maintenance for
- tele: Is the Telephone registered or not
- foreign: Is the applicant a foreign worker

LOGISTIC REGRESSION OUTPUT:

![image](https://user-images.githubusercontent.com/117341679/221497087-d47f92ae-24f8-48e7-9605-f204ca35c8d5.png)

DECISION TREES OUTPUT:

![image](https://user-images.githubusercontent.com/117341679/221497186-bb31b7a1-f069-4e5f-9c5f-8dd96902f12b.png)

![image](https://user-images.githubusercontent.com/117341679/221497246-23c85685-4d6b-4ab2-9f41-572b58d6f30c.png)

RANDOM FOREST OUTPUT:

![image](https://user-images.githubusercontent.com/117341679/221497373-751fe690-06d3-4549-a1d7-aa5dc8c94d5c.png)

SUPPORT VECTOR MACHINE(SVM):

![image](https://user-images.githubusercontent.com/117341679/221497451-d6c816ee-ed73-443c-87f3-0d976d56a533.png)

MODEL DEPLOYMENT:

Based on the above trials you select that algorithm which produces the best average accuracy. In this case, multiple algorithms have produced similar kind of average accuracy. Hence, we can choose any one of them.I am choosing SVM as the final model since it is very fast on this high dimensional data.

Flask is a lightweight web framework for Python that can be used to build and deploy web applications, including machine learning models. Here are the general steps to deploy a loan prediction model using Flask:

- Train and save the model: You first need to train a machine learning model on a loan prediction dataset and save the model to a file using a serialization library like pickle or joblib.

- Create a Flask app: You can create a Flask app that defines a route to handle loan prediction requests. The app should load the trained model from the saved file and use it to make predictions on new loan applications.

- Deploy the Flask app: You can deploy the Flask app to a server or cloud platform that supports Python web applications. There are many options for deployment, including Heroku, AWS Elastic Beanstalk, and Google Cloud App Engine.


