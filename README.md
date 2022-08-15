# Neural_Network_Charity_Analysis
## Purpose
### A company that funds non-profit work is trying to determine whether or not applicants will be successful in their endeavors if they receive funding from the philanthropic company. In short, this is a loan prediction risk analysis. To do this, a large dataset (34,000 organizations) of previous recipients of the philanthropic company's funding was compiled and a neural network model was created. If the model can be optimized to predict success of applicants by over 75%, then the philanthropic company will be better suited to fund the organizations most likely to succeed.

## Results
### Data Preprocessing
#### Target Variable is "IS_SUCCESSFUL"
#### Features are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT
#### Variables that should be removed are EIN, NAME, SPECIAL_CONSIDERATIONS, and STATUS
### Compiling, Training, and Evaluating the Model
#### For the original neural network model, I chose 2 hidden layers each using the "relu" activation function. The first hidden layer had 10 neurons, and the second hidden layer had 5 neurons. I chose these because they were the examples given in class and I figured it was as good a place to start as any. The same reasoning goes for the activation functions.
#### I was not able to achieve the target model performance.
#### I increased the neurons, increased the hidden layers, changed the activation functions on the layers, and removed SPECIAL_CONSIDERATIONS, and STATUS from the features list.

## Summary
### The models all had a low accuracy score and a relatively high loss score. 
### Original NN Model
![image](https://user-images.githubusercontent.com/102757676/184563428-6e531866-db07-4d4d-9867-409031e5fdfc.png)

### Optimization 1
![image](https://user-images.githubusercontent.com/102757676/184563330-ab97e0fc-ea6a-4192-93d1-52f7d2632ce1.png)

### Optimization 2
![image](https://user-images.githubusercontent.com/102757676/184563377-99da8b3e-a9af-4bc1-a7b7-41ff1e709b31.png)

### Optimization 3
![image](https://user-images.githubusercontent.com/102757676/184563384-fa31fddc-de0c-424c-87a7-1bd652281e11.png)


### I would suggest trying to use an SVM model instead of a basic neural network model because it can classify and create regression using two groups really well. Since this problem was to classify loan applications as likely to succeed and unlikely to succeed, SVM would work for this binary classification. Furthermore, SVMs are less prone to overfitting and can look at the bigger picture much better than neural network models.
