# Horizont
This capstone project for Duke University’s “AI Product Management” course on Coursera represents my first work in data segmentation and marks my entry into the AI field. I am grateful to my boyfriend for his encouragement, which has given me the confidence to explore my potential more fully.

### **Mission**
In this project you will have an opportunity to apply your new knowledge of the modeling process to develop a machine learning model to solve a simple problem.  You will be provided a small dataset and your task will be to perform the basic steps of the **modeling process to train and evaluate a machine learning model on the dataset**.  Your final deliverable for this project is a short (5 minutes maximum) presentation video **describing your approach to building the model, sharing a brief demo/screenshot of your model, and describing how you have decided to evaluate your final model**. 

This project will be peer graded.  Your peers will evaluate your video presentation for the following four elements:

1. **Modeling approach** - did you correctly identify the type of modeling task, features to use, and possible algorithms to use?
2. **Model building**  - did you compare at least two different models (different algorithms, different combinations of features, or different hyperparameter combinations) using a vlidation set or cross-validation to optimize your model?
3. **Model evaluation** - did you set a reasonable evaluation metric to determine the performance of your model, and then calculate it on the test set?
4. **Model interpretation** - did you correctly interpret and clearly communicate the performance of your model?
### **Project topic:**

In this project we will build a model to predict the electrical energy output of a [Combined Cycle Power Plant](https://en.wikipedia.org/wiki/Combined_cycle_power_plant), which uses a combination of gas turbines, steam turbines, and heat recovery steam generators to generate power.  We have a set of 9568 hourly average ambient environmental readings from sensors at the power plant which we will use in our model.

The columns in the data consist of hourly average ambient variables: - Temperature (T) in the range 1.81°C to 37.11°C, - Ambient Pressure (AP) in the range 992.89-1033.30 milibar, - Relative Humidity (RH) in the range 25.56% to 100.16% - Exhaust Vacuum (V) in the range 25.36-81.56 cm Hg - Net hourly electrical energy output (PE) 420.26-495.76 MW (Target we are trying to predict)

### **Guidelines for the project:**

To complete the project, you must complete each of the below steps in the modeling process.  

1. For the problem described in the Project Topic section above, determine what type of machine learning approach is needed and select an appropriate output metric to evaluate performance in accomplishing the task.
2. Determine which possible features we may want to use in the model, and identify the different algorithms we might consider.
3. Split your data to create a test set to evaluate the performance of your final model.  Then, using your training set, determine a validation strategy for comparing different models - a fixed validation set or cross-validation.  Depending on whether you are using Excel, Python or AutoML for your model building, you may need to manually split your data to create the test set and validation set / cross validation folds.
4. Use your validation approach to compare at least two different models (which may be either 1) different algorithms, 2) the same algorithm with different combinations of features, or 3) the same algorithm and features with different values for hyperparameters).  From among the models you compare, select the model with the best performance on your validation set as your final model.
5. Evaluate the performance of your final model using the output metric you defined earlier.  

==========

This script demonstrates the complete workflow for modeling the electrical energy output (PE) of a Combined Cycle Power Plant:

1. Data loading and initial exploration  
2. Definition of features and target variable  
3. Dataset splitting: training set and test set (80%-20%)  
4. Validation strategy: 5-fold cross-validation  
5. Model comparison: Linear Regression vs. Random Forest Regression  
6. Training of the best-performing model and evaluation on the test set (MSE)  
7. Visualization of results
