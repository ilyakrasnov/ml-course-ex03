<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=TeX-AMS-MML_HTMLorMML"></script>

# Finding Best Features (Ex 03)
##### Machine Learning Course @JCE - by Ilya Krasnov (341008159)

### Project Scope and Description
Given a dataset input in form of an Excel spreadsheet, a logistic regression algorithm was implemented from scratch. The algorithm was trained on the first 300 rows of the dataset and tested on the remaining rows.

### Tools and Implementation
The algorithm was implemented in Python, using Pandas for data frame manipulation as well as seaborn and matplotlib for visualisation.
For convenience, the project was implemented using a jupyter notebook. The notebook as well as this report are under version control and can be found on [github][1]

### Implemented Algorithm

### Results

#### Definition of Accuracy

The accuracy was defined by the following formula:

\\[ { {CorrectPredictions} \over {TotalPredictions} } \times 100 \\]

#### Training Accuracy
The following accuracy results were produced with 100 iterations of the gradient descent and different alpha values. For all cases the final accuracy of nearly

$$  98\% $$

was achieved.


##### alpha = 0.2
![](training_quality_0.png )

##### alpha = 0.03
![](training_quality_1.png )

##### alpha = 0.02
![](training_quality_1_1.png )

##### alpha =  0.01
![](training_quality_2.png )

##### alpha =  0.003
![](training_quality_3.png )

#### Test Accuracy
The accuracy for the test data using the final \\(\theta\\) was: $$ 97.77\% $$

### Conclusion

We clearly see that finding the right \\(\alpha\\) values is very important. With the initial value of 0.2 we can see fluctuations in the accuarcy, although with overall trend towards 100%. Making \\(\alpha\\) smaller produces much nicer results. With \\(\alpha = 0.02\\) we see a fast convergence, almost after 10 interations. Making \\(\alpha\\) too small on the other hand lets the alogirthm converge slower, thus making a higher number of iterations necessary in order to achieve high accuracy values.


[1]:	https://github.com/ilyakrasnov/ml-course
