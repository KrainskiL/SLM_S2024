## Competition rules
### Teams
Teams should consist of 1-3 members. Please name the team - name will appear in the results table (can be anything you come up with but please avoid PII data in the group name e.g. surnames).

### Dataset and competition's goal
Goal of the competition is to achieve highest:
* Groups 11 and 13 - **[F1-score](https://en.wikipedia.org/wiki/F-score)**
* Group 12 - **accuracy**

in classification of target variable **IsIPA**. To create a model please use **IPA.csv** dataset (used it for both train and validation dataset) and predict labels on **IPA_test.csv** data. Description of dataset features can be found in **IPA_description.txt**.

### Results delivery
Please send the results to _lkrain@sgh.waw.pl_ by the end of the class.

In the e-mail please specify name of the group and members (only one mail per group is required). Required attachments are:
1. R/Python/Julia script or notebook with used code
2. CSV file named **[group_name]_IPA_prediction.csv** with one column named **Prediction** containing 5000 predictions with values 1/0 or TRUE/FALSE for dataset **IPA_test.csv**. Please make sure predictions order is the same as rows in test data.

Please check whether the ordering of predictions is consistent with the observations in test set. Please pay attention to missing data in the test set - they must be properly handled to obtain exactly 5000 predictions.

Table with ranking will appear in this README file. Best team in each course group will receive 5 points, next 4 points, etc.

Good luck!

## Results

Group 13 (class at 9:50)

| **Team**          | **F1-score** | **Points** | **Model** | **Language**              |
|---------------------|--------------|------------|-----------|------------------------|
| Idea Squad             | 78,96 | 5 | Random Forest           | Python |
| Random Experts         | 78,72 | 4 | ?                       | ?      |
|  Big Head & Little Pig | 78,67 | 3 | Random Forest           | Python |
| ML Dream Team          | 76,73 | 2 | XGBoost (Boosted Trees) | Python |
| Gucci                  | 70,31 | 1 | Logistic Regression     | Python |

Group 11 (class at 11:40)

| **Team**          | **F1-score** | **Points** | **Model** | **Language**              |
|---------------------|--------------|------------|-----------|------------------------|
| 2Slavs       | 78,58 | 5 | Random Forest       | Python |
| Data Wizards | 78,54 | 4 | Random Forest       | Python |
| Alpha        | 76,39 | 3 | CART                | Python |
| Big Mac      | 66,24* | 2 | Logistic Regression | Python |
| NAM          | ?     | 1 | CART                | Python |
| Group 1      | ?     | 1 | Deep Neural Network | Python |

\* first 5000 predictions used in evaluation
