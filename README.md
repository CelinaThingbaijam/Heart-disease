# Heart-disease
It is a classification data in which we predict if someone will have heart disease or not depending upon their
1) age
2)sex
3)Constrictive pericarditis(CP) - A form of diastolic heart failure that arises because an inelastic pericardium inhibits cardiac filling
4)trestbps (Resting blood pressure)
5) chol (Cholesterol level)
7) fbs(fasting blood sugar) -if >120 1 = True,0 = False
8) restecg(Resting electrocardiographic measurement) -0= normal,1 = having ST-T wave abnormality,2 = hypertrophy
9)thalach - Person maximum heart rate
10) Exang( Exercise Induced angina) -- 0=no,1 = yes
11) oldpeak : ST depression induced by exercise relative to rest
12)Slope : ST/heart rate slope
13)ca : Calcium present or not (Higher the score higher will be the risks)
14)thal: People with thalassemia can get too much iron in there bodies which may lead to heart disease
15) target : heart disease no = 0,heart disease yes = 1
After analysis the data
we do eda( Exploratory data analysis)
-on checking we get to find that there is no null value and all the data is either float and integer
-then start apply the classification algorithms ( on checking we find that LogisticRegression has the best result (81.9%)
- we try to improve the data by preprocessing using StandardScaler in pipelines.
As a result we got to see some significant improvement in KNN (65 to 81.4) and SVC( 64 to 73.5)
- As we saw some significant improvement in KNN and SVC we want see if their accuracy will improve or not using GridSearchCV.
for KNN we got (84.1 ,neighbors = 11) and for SVC we got (82.22 ,kernel ="rbf")
Lastly ,we want want to check with all the ensembles techniques to see if there is any better accuracy then KNN.
On checking we didn't find any accuracy better than KNN
So KNN was the Algorithms which give an accuracy of 86.3
