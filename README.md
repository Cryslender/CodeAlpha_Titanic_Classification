# Titanic Classification Project
## 1. Introduction
This project aimed to predict the likelihood of a person's survival in the Titanic disaster and to identify the socio-economic factors that contributed to their survival. The following structured approach was used to achieve this objective.

## 2. Ask Question
The analytical process begins with a question to be answered. In this project, the central question is: "What are the contributing factors to a person's survival in the Titanic sinking?"

## 3. Get Data
This step involves locating and obtaining relevant data, followed by assessing if there is enough data to perform the analysis. For this project, the training and testing data were acquired from Kaggle.

## 4. Investigate Data
Data can come in various forms and from multiple sources. This step involves assessing if the data is complete and contains the necessary information for analysis.

## 5. Prepare Data
This phase, also known as "data cleaning," involves transforming the data into a suitable format for analysis. This includes rectifying issues such as missing values and obvious errors to ensure the data is ready for analysis. In this project, the following steps were taken:

* Checked the shape of the data to understand the number of columns and rows.
*Verified column names to ensure the data was suitable for answering the project question.
* Verified column data types to ensure correctness.
* Checked for null values and found missing data in the Age, Fare, Cabin, and Embarked columns.
* Handled missing values by:
  1. Replacing missing values in Age and Fare with the mean of each column.
  2. Filling missing values in Cabin with the word "Unknown."
  3. Filling missing values in Embarked with the mode of the column.
* Checked for duplicates and confirmed there were no duplicate rows.
* Identified the unique values in the dataset.
* Obtained data information to understand its structure and types.
* Generated a statistical summary to understand the distribution of numerical data.
* Counted the values of non-survivors and survivors to check for data balance.
## 6. Feature Engineering
This step involves creating new columns and deleting unnecessary ones:

* Created the "Title" column from the "Name" column.
* Deleted the "Name" column.
* Created the "Deck" column from the "Cabin" column and then deleted the "Cabin" column.
* Deleted the "Ticket" column.
* Created the "Family Size" column.
* Created the "Fare Group" column (used only for analysis and then deleted).
* These steps ensured that the data was clean, organized, and ready for further analysis.

## 7. Analyze Data
This step involves exploratory data analysis (EDA) to gain more insight from the data. Visualization tasks are used to uncover patterns, correlations, and relationships, allowing for a deeper understanding of the data.

## 8. Preprocessing
To predict whether a person would survive the sinking, the project applied an Ordinal Encoder to convert categorical variables to numeric values suitable for machine learning. The training data was split into independent and dependent variables and further divided into training (80%) and validation (20%) sets.

## 9. Model Design
This step involves designing the structure of the model. A Random Forest Classifier was used for this project.

## 10. Model Training
In this phase, the model was trained on the training dataset and validated on the validation data, achieving an 85% accuracy rate.

## 11. Model Testing
The model was evaluated on clean and processed testing data to predict whether a person would survive the sinking. A "Survived" column was created from these predictions.

## 12. Socio-Economic Factors
The project used feature importance to identify the socio-economic factors that contributed to survival. The top five factors identified were Sex, PassengerID, Fare, Age, and Title.
