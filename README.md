# Portuguese Bank :
To create a predictive model which will help the bank marketing team to know which customer will buy the product.

This dataset is about the direct phone call marketing campaigns, which aim to promote term deposits among existing customers, by a Portuguese banking institution from May 2008 to November 2010. 

The objective of this project is to analyze the dataset's result of past bank telemarketing campaign and perform machine learning algorithms for predicting valuable customers who will join a term deposit product. The dataset was taken from 2008 to 2013 and it had an imbalance data with the majority of negative result distribution. As the bank's data scientists, we decided to focus on minimizing False Negative Class.

Evaluation metric that we will use is Recall. Where we will minimize false negative class - where we predicted clients that will not open a term deposit, turns out they actually want to open a term deposit. As our objective is to have as many clients to open a term deposit, therefore increasing recall will decrease this type of error.

The main goal of this project was to be able to predict which customers would subscribe to a term deposit for Bank Of Portugal. The project uses data collected by the Bank of Portugal that includes customers profiles of those who have subscribed to term deposits and the ones who did not subscribe to a term deposit.

The deep explanatory analysis has shown the dataset is a victim of high class imbalance. It also showed that day_of_week doesn’t help much in the prediction.

After the EDA, the dataset was preprocessed by using a one-hot encoder for categorical variables whereas, StandardScaler was used for numerical columns.

Then we created pipelines consisting of 5 classifiers to be compared by the use of f1 score,recall_score,precision_score

# Bussniess  case
case 1 : Customers with high chances of buying the product but the model predicted them as customers who are not interested in buying the product. 

case 2 : Customers with low chances of buying the product but the model predicted them as customers who are highly  interested in buying the product 

Both case 1 and case2 are problematic, so recall and precision both scores should be high.

# Models used :
Logistic reggression ,KNN, SVM, Desicion Tree, Random Forests


# Result Table :
                              
                               Recall_score         Precision_score        f1_score      Accuracy_score
    
     Logistic reggression           0.84                 0.83                   0.83              0.84

            KNN                     0.99                  0.81                  0.89              0.88
            
            SVM                     0.76                  0.75                  0.76              0.76
            
     Desicion Tree                 0.91                  0.79                  0.85              0.83
    
    Random Forests                  0.95                  0.90                  0.92              0.92
    
    
# Result:Random Forest has the recall with 95% and precision score of 90%, Random Forest predicted is giving more precised score then other algorithms.
    
