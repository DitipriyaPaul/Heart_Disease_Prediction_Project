# Heart_Disease_Prediction_Project
# Introduction 
According to the World Health Organization, Cardiovascular diseases (CVDs) are the number 1 cause of 
death globally: more people die annually from CVDs than from any other cause. An estimated 17.9 
million people died from CVDs each year. Of these deaths, 85% are
due to heart attack and stroke. The high mortality rate and expensive surgery cost already make heart 
disease become a serious threat for many families in many parts of the world, especially those poor stricken countries. Therefore, it is crucial for people to analyze the relationship between various kinds of 
attributes in human and the possibility of suffering from heart disease. A robust model is helpful and 
meaningful in predicting which type of people is more likely to have a heart disease thus we can prepare 
or prevent in advance. 
Machine learning is closely related to computational statistics, which focus on using mathematical 
optimization to deliver methods, theory and application domains to solve medical, industry, social and 
business problems in the real world. It can be divided into two broad categories: supervised learning and 
unsupervised learning. In supervised learning, the algorithm builds a mathematical model from a set of 
data that contains both the inputs and the desired outputs. While in unsupervised learning, the algorithm 
builds a mathematical model from a set of data that contains only inputs and no desired output labels.
Since our objective is to predict the possibility of having heart disease based on the physical body 
function. And inputs and desired outputs are expected, definitely we should choose the supervised 
learning. In this thesis, I would use four models (logistic regression, random forest, extreme gradient 
boosting and neural network) in supervised learning to predict the possibility of people to have heart 
disease based on people’s physical function of the body. 
To fulfill the objective of my thesis, the following steps may be followed. 
1. Download the data set “Heart Disease” from UCI Machine Learning Repository webpage
2. Clean the data and perform exploratory data analysis
3. Apply four different models 
4. Compare the results of these four models
5. Draw conclusion based on the result

# Project_Objective
This data set is obtained from UCI Machine Learning Repository webpage. It contains 76 attributes, but 
all published experiments refer to using a subset of 14 of them. The total observations are 303. And it 
was donated by David W. Aha.
# Attribute_Information
AGE: age in years
SEX: (1 = male; 0 = female)
CP (Chest Pain Type): 
--Value 0: typical angina (most serious)
--Value 1: atypical angina
--Value 2: non-anginal pain
--Value 3: asymptomatic (least serious)
TRESTBPS: resting blood pressure (in mm Hg on admission to the hospital)
CHOL: serum cholesterol in mg/dl
FBS: (fasting blood sugar > 120 mg/dl) (1 = true; 0 = false)
A fasting blood sugar level less than 100 mg/dL is normal. From 100 to 120 mg is considered 
prediabetes. If it is 125 mg/dL or higher on two separate tests, you have diabetes.
4
RESTECG (Resting Electrocardiographic Results):
--Value 0: normal
--Value 1: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 
0.05 mV)
--Value 2: showing probable or definite left ventricular hypertrophy by Estes' criteria
THALACH: maximum heart rate achieved
EXANG: exercise induced angina (1 = yes; 0 = no)
OLDPEAK: ST depression induced by exercise relative to rest
SLOPE (the slope of the peak exercise ST segment):
--Value 0: upsloping
--Value 1: flat
--Value 2: downsloping
CA: number of major vessels (0-3) colored by fluoroscopy
THAL: 3 = normal; 6 = fixed defect; 7 = reversable defect
TARGET: diagnosis of heart disease (angiographic disease status)
-- Value 0: < 50% diameter narrowing
-- Value 1: > 50% diameter narrowing
(in any major vessel: attributes 59 through 68 are vessels


# Project_Overview
There are two variables playing significant roles in predicting the dependent variable “Target”. That is 
“trestbps” (resting blood pressure) and “thalach” (maximum heart rate achieved).
Usually we use blood pressure readings to analyze and monitor blood pressure. These tests record blood 
pressure using two measurements: systolic and diastolic blood pressure. According to the research, both 
high systolic and high diastolic blood pressure can lead to heart attack and stroke.
On the other hand, I have also found many reports said that a high heart rate was associated with a 
higher risk of all-cause mortality and cardiovascular events. It has also been proven that the relationship 
tends to be stronger in women than men.  
Some people may tend to believe that blood pressure has nothing to do with heart rate. However, the fact 
is that the acceleration of heart rate is closely correlated with the increasing risk of the cardiovascular 
system. The heart rate for normal person is 60 to 100 times one minute. The rise of heart rate mostly 
results from sympathetic activation, which has reciprocal causation with high blood pressure. In a 
nutshell, when we have a racing heart, the risk of hypertension is higher. On the other hand, high blood 
pressure can also result in functional damage to our heart, and further accelerates our heart rate. 
Aside from the two common variables, we should also pay much attention to cp (chest pain), thal and ca
(number of major vessels colored by fluoroscopy). 
Chest pain, also called angina, is caused when your heart muscle doesn't get enough oxygen-rich blood. 
It may feel like pressure or squeezing in your chest. The discomfort also can occur in your shoulders, 
arms, neck, jaw, or back. Angina pain may even feel like indigestion. Angina can also be a symptom of 
coronary microvascular disease. This is heart disease that affects the heart’s smallest coronary arteries 
and is more likely to affect women than men . This research confirms what we have found in 
exploratory data analysis . Hence when we feel angina, we may first take heart disease into 
consideration and go to the hospital as soon as possible.
While thal (thalassemia), is an inherited blood disorder that causes your body to have less hemoglobin 
than normal. Thalassemia can cause anemia, leaving you fatigued. Untreated anemia, in which 
hemoglobin levels are consistently too low, often causes tachycardia, as the heart tries to compensate for 
the lack of oxygen being carried through the body. Over time, the heart also becomes enlarged [10]. 
Hearts are unavoidably affected by thalassemia. Hence when people are diagnosed with thalassemia, 
they may check their body regularly to prevent emergent problems with heart. 
When it comes to the X-ray fluoroscopy, we cannot deny its magical function to guide vascular and 
cardiac interventions, especially in real-time imaging and easy access to patients during interventions. 
But each coin has two sides, X-ray fluoroscopy is limited for defining soft tissue and obtaining 
functional information, regardless of the evidence that exposure to ionizing radiation from X-ray 
procedures is associated with an increased risk of cancer. People may be more cautious with X-ray 
fluoroscopy, take advantage of its major function and keep updating the technology. And I believe in the 
foreseeable future, X-ray fluoroscopy will be more flexible, accurate and safe for people to use.
The good news, however, is that 80% of premature heart attacks and strokes are preventable. Healthy 
diet, regular physical activity, and not using tobacco products are the keys to prevention. Checking and 
controlling risk factors for heart disease and stroke such as high blood pressure, high cholesterol and 
high blood sugar or diabetes is also very important.
We can also take the following actions to prevent heart disease. 
1. Eat a healthy diet.
2. Take regular physical activity.
3. Avoid tobacco use.
4. Check and control your overall cardiovascular risk
