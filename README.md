# Titanic-Kaggle
A machine learning algorithms using Titanic Dataset

## The Challenge from Kaggle
> The sinking of the Titanic is one of the most infamous shipwrecks in history.
> On April 15, 1912, during her maiden voyage, the widely considered “unsinkable” RMS Titanic sank after colliding with an iceberg. Unfortunately, there weren’t enough lifeboats for everyone onboard, resulting in the death of 1502 out of 2224 passengers and crew.
> While there was some element of luck involved in surviving, it seems some groups of people were more likely to survive than others.
> In this challenge, we ask you to build a predictive model that answers the question: “what sorts of people were more likely to survive?” using passenger data (ie name, age, gender, socio-economic class, etc).

### 1) Understanding the data
For this part I use the famous library in python which is pandas (Python Data Analysis Library)

i) df.info 
   - To get the info about the data
   - We also can get the information about missing value or null value
   
ii) df.describe
   - To get the central tendency of the data (mean, mode, median, min, max and etc.)
   
### 2) Light Data Exploratory Analysis
For this part I use seaborn and matplotlib library
- I look the distribution for categorical and numerical data
- Here are some pivot table and graph we  can get from the titanic dataset\

![Pivot table](https://user-images.githubusercontent.com/77544994/106116176-92bb5b80-618c-11eb-82e9-1c758fa2e477.PNG)
![survived](https://user-images.githubusercontent.com/77544994/106116364-c8f8db00-618c-11eb-96f9-c2064c7ed484.PNG)
![Pclass](https://user-images.githubusercontent.com/77544994/106116498-ef1e7b00-618c-11eb-8ce2-a997f9398712.PNG)
![age](https://user-images.githubusercontent.com/77544994/106116782-47ee1380-618d-11eb-9dbe-0031c635670c.PNG)

### 3) Data Cleaning
There is some null value in Titanic dataset
- Train Data
  - Age
  - Cabin
  - Embarked
  
- Test Data
  - Age
  - Cabin 
  - Fare
  
For age column, I fill the null value with its mean\
For Embarked column, I fill the null value with its mode\
For Fare column, I fill the null value with its median\
lastly, I choose to drop the Cabin column\

- I also do some features engineering to:
  - Name
  - Sex
  - Age
  - SibSp + Parch
  - Fare
  - Embarked
  
### 4) Model Selection
I choose 5 different models for this machine learning project:
- Decision Tree 
- Random Forest
- KNN
- Logistic Regression
- Support Vector machine

![score](https://user-images.githubusercontent.com/77544994/106119040-b46a1200-618f-11eb-86f5-16b1a79ee838.PNG)
