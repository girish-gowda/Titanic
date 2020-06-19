# Titanic
imported libraries numpy, pandas, matplotlib.pyplot and seaborn

#Titanic Dataset download link
https://www.kaggle.com/c/titanic/data

Test(Except Survived) and Train Dataset contains below columns:
 0   PassengerId  891 non-null    int64  
 1   Survived     891 non-null    int64  
 2   Pclass       891 non-null    int64  
 3   Name         891 non-null    object 
 4   Sex          891 non-null    object 
 5   Age          714 non-null    float64
 6   SibSp        891 non-null    int64  
 7   Parch        891 non-null    int64  
 8   Ticket       891 non-null    object 
 9   Fare         891 non-null    float64
 10  Cabin        204 non-null    object 
 11  Embarked     889 non-null    object

#Droped columns "PassengerId", "Name", "Ticket"

#Drop the column containing more missing cells

#Column accepting only numeric values, replace the empty cells with mean of values
#Column accepting only categorical values, replace the empty cells with mode of values

Now the Data is ready to use for Model Creation using Classification Algorithm

I have tried for best possible fit using cleaned data with below algorithms:

from sklearn.ensemble import RandomForestClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.tree import DecisionTreeClassifier
from sklearn.neighbors import KNeighborsClassifier

RandomForestClassifier has providing 98.2% accuracy rate and submitted on kaggle competition

This code in kaggle competition rank is 4681/24741
