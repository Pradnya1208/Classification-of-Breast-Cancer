<div align="center">
  
[1]: https://github.com/Pradnya1208
[2]: https://www.linkedin.com/in/pradnya-patil-b049161ba/
[3]: https://public.tableau.com/app/profile/pradnya.patil3254#!/
[4]: https://twitter.com/Pradnya1208


[![github](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c292abd3f9cc647a7edc0061193f1523e9c05e1f/icons/git.svg)][1]
[![linkedin](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/9f5c4a255972275ced549ea6e34ef35019166944/icons/iconmonstr-linkedin-5.svg)][2]
[![tableau](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/e257c5d6cf02f13072429935b0828525c601414f/icons/icons8-tableau-software%20(1).svg)][3]
[![twitter](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c9f9c5dc4e24eff0143b3056708d24650cbccdde/icons/iconmonstr-twitter-5.svg)][4]

</div>

# <div align="center">Building a Simple Machine Learning Model on Breast Cancer Data</div>
<div align="center">
<img src = "https://github.com/Pradnya1208/Tree-based-Models-for-the-classification-of-Breast-Cancer/blob/main/output/intro.jpg?raw=true" width="80%">
</div>

## Overview:
Breast cancer is one of the most common cancers among women worldwide, representing the majority of new cancer cases and cancer-related deaths according to global statistics, making it a significant public health problem in today’s society.

The early diagnosis of it can improve the prognosis and chance of survival significantly, as it can promote timely clinical treatment to patients. Further accurate classification of benign tumors can prevent patients undergoing unnecessary treatments. Thus, the correct diagnosis of Breast Cancer and classification of patients into malignant or benign groups is the subject of much research. Because of its unique advantages in critical features detection from complex Breast Cancer datasets, machine learning (ML) is widely recognized as the methodology of choice in Breast cancer pattern classification and forecast modelling.
Classification and data mining methods are an effective way to classify data. Especially in medical field, where those methods are widely used in diagnosis and analysis to make decisions.

Because we are categorizing whether the tissue is cancerous or benign, we will train multiple Tree-based models for this procedure. We’ll experiment with hyper-parameters to see if we can enhance the accuracy. Try to solve the problem using the approach outlined below. For further information on each feature, consult the data dictionary.
Decision trees (DTs) form the basis of ensemble algorithms in machine learning.
These are powerful algorithms that can fit complex data. 

In this project, our focus is on understanding the core concepts of the Decision Tree for healthcare analysis, followed by understanding the different ensemble techniques.


## Dataset:
[Breast cancer wisconsin (diagnostic) dataset](https://scikit-learn.org/stable/datasets/toy_dataset.html#breast-cancer-dataset)
```
from sklearn.datasets import load_breast_cancer
X,y = load_breast_cancer(return_X_y=True, as_frame=True)
```

### Data Set Features:
- radius (mean of distances from center to points on the perimeter)
- texture (standard deviation of gray-scale values)
- perimeter

- area

- smoothness (local variation in radius lengths)

- compactness (perimeter^2 / area - 1.0)

- concavity (severity of concave portions of the contour)

- concave points (number of concave portions of the contour)

- symmetry

- fractal dimension (“coastline approximation” - 1)
- class: Malignant or Benign


### Implementation:

**Libraries:**  `NumPy` `pandas` `pylab` `matplotlib` `sklearn` `seaborn` `plotly`

#### Count of Malignant(value =0) and Benign(value = 1) tumors:
<img src ="https://github.com/Pradnya1208/Classification-of-Breast-Cancer/blob/main/output/Capture.PNG?raw=true">

Data has no nyll values, but we have removed some highly correlated features:
```
drop_list = ['mean perimeter','mean radius','mean compactness','mean concave points','radius error','perimeter error','compactness error','concave points error','worst radius','worst perimeter','worst compactness','worst concave points','worst texture','worst area']
X = X.drop(drop_list, axis=1)
```

## Machine Learning Model Evaluation and Prediction:
We have used following models for classification:
#### Decision trees classifier:
```
The accuracy of the model is: 95.61
confusion matrix
[[40  3]
 [ 2 69]]
```

#### Logistic Regression
```
The accuracy of the model is: 97.37
confusion matrix
[[42  1]
 [ 2 69]]
 ```

#### KNN classifier:
```
The accuracy of the model is: 92.11
confusion matrix
[[38  5]
 [ 4 67]]
```

#### SVM:
```
The accuracy of the model is: 97.37
confusion matrix
[[42  1]
 [ 2 69]]
```

#### K-SVM:
```
The accuracy of the model is: 92.98
confusion matrix
[[38  5]
 [ 3 68]]
```

#### Naive Bayes:
```
The accuracy of the model is: 93.86
confusion matrix
[[39  4]
 [ 3 68]]
 ```

#### Random Forest:
```
The accuracy of the model is: 95.61
confusion matrix
[[41  2]
 [ 3 68]]
 ```



### Lessons Learned
`Classification Algorithms`
`Scaling and Data Transformation`






## References:
[Building a Simple Machine Learning Model on Breast Cancer Data](https://towardsdatascience.com/building-a-simple-machine-learning-model-on-breast-cancer-data-eca4b3b99fa3)
### Feedback

If you have any feedback, please reach out at pradnyapatil671@gmail.com


### 🚀 About Me
#### Hi, I'm Pradnya! 👋
I am an AI Enthusiast and  Data science & ML practitioner


[1]: https://github.com/Pradnya1208
[2]: https://www.linkedin.com/in/pradnya-patil-b049161ba/
[3]: https://public.tableau.com/app/profile/pradnya.patil3254#!/
[4]: https://twitter.com/Pradnya1208


[![github](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c292abd3f9cc647a7edc0061193f1523e9c05e1f/icons/git.svg)][1]
[![linkedin](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/9f5c4a255972275ced549ea6e34ef35019166944/icons/iconmonstr-linkedin-5.svg)][2]
[![tableau](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/e257c5d6cf02f13072429935b0828525c601414f/icons/icons8-tableau-software%20(1).svg)][3]
[![twitter](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c9f9c5dc4e24eff0143b3056708d24650cbccdde/icons/iconmonstr-twitter-5.svg)][4]
