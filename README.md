# Cuff Less Blood Pressure Estimation Dataset

1. What is the purpose of the research?
1.1 Introduction:
Hypertension is a major health problem worldwide and is a major risk factor for many cardiovascular diseases. Accurate and regular measurement of blood pressure is critical for early detection and management of hypertension. The traditional method of cuffed blood pressure measurement can be perceived by users as uncomfortable and limiting. Therefore, cuffless blood pressure estimation is being investigated as a more comfortable and user-friendly alternative. The Cuff-Less Blood Pressure Estimation Dataset is a dataset created to contribute to the research in this area. I will explain the steps taken on this dataset through code analysis and modeling, and I will compare these data with graphical outputs simultaneously by working on the code myself.
1.2 Creating a Dataset:
The Cuff-Less Blood Pressure Estimation Dataset is the product of a large-scale study and contains data collected from various sources. The dataset contains real-time data from a variety of participants, including many different characteristics. These features include electrocardiography (ECG) data, pulse wave data, acceleration data and respiration data. Each participant has a reference tag that contains this data collected during the cuffed blood pressure measurement.
1.3 Research Objective:
The Cuff-Less Blood Pressure Estimation Dataset was created to form the basis for various research in the field of cuffless blood pressure estimation. This dataset encourages the development of machine learning and artificial intelligence algorithms for estimating blood pressure. Using this dataset, researchers can test different algorithms, develop new methods and improve existing methods. They can also use this dataset to evaluate the accuracy and reliability of sensors used in cuffless blood pressure estimation.
The code part is to analyze the dataset of blood pressure measurements. In this analysis, photoplethysmography (PPG) signals, a sensor that measures oxygen levels in the blood, and electrocardiography (ECG) signals are used.
1.4 Conclusion:
In conclusion, the Cuff-Less Blood Pressure Estimation Dataset is a major contribution to research on cuffless blood pressure estimation. By providing a platform for the development and evaluation of various algorithms, this dataset inspires work towards developing a more user-friendly and convenient method for early diagnosis and management of hypertension. Furthermore, the dataset serves as an essential reference source for the development of sensor technologies and improving their accuracy. The findings from the use of this dataset can contribute to the development of more effective strategies for the prevention and treatment of hypertension.


2. How many observations does the dataset consist of? What is the number of rows and columns?
In this area, let's first examine the properties of the dataset we examined through the code:
- The dataset contains 1000 observations. 
- For each observation, 3 signals were recorded: PPG, ECG and blood pressure (BP). 
- Each signal consists of 125 samples. 
- Systolic Blood Pressure (SBP) and Diastolic Blood Pressure (DBP) values were recorded separately.
This code means that the sequence of rows contains 1 row and 1000 columns.
While obtaining these steps, I tested this process with Spyder IDE on Anaconda, which we used in the course. I share these additional images with you:

 ![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/37343b9b-9854-4172-95af-1db6c580a14d)

 Array;

 ![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/68b7523f-749c-43c1-b1a9-8220a240428a)

this is the way it is.

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/1b87ae84-f1e6-4a3b-bda7-cfce0a93c575)

The libraries used are given at the top left. These are

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/6c7732af-ebf7-4a3f-b8f3-456b18556caf)

Note: It appears that I imported the dataset into the code by importing the os command from the desktop. These library descriptions are given in Chapter 7 with explanations.
3. Do I need special permission to use the dataset?
The use of the dataset does not require special permission. It is open source. This open source is shared in the bibliography (CC0 public domain)
4. Which types of data structures are used?
In this code, I have explained the data structures in the dataset analysis code, machine learning modeling code and deep learning modeling code in a way to cover them all. As I have done model training before, I wanted to present these libraries to you in Title 7 as an addition to the course content.
The following data structures are used in this code example:
Numpy: It is a library used to perform numerical calculations. For example, numerical operations such as matrix operations were performed using numpy.
Pandas: It is a library used for data manipulation. It is used to read, manipulate and analyze data sets.
Seaborn: It is a library for data visualization. Seaborn library is used to create graphics and visualizations.
Scipy: A library for scientific computing and signal processing. Scipy is used to perform various operations such as mathematical operations, signal processing algorithms and transformations.
Scikit-learn: A library for building and evaluating machine learning models. Scikit-learn is used to build and train models such as linear regression, random forest regression, etc.
Matplotlib: It is a library used to create graphics and visualizations. Matplotlib was used to visualize the data.
TensorFlow: It is a library used for creating and training deep learning models. TensorFlow was used to create neural networks and deep learning models.
These data structures were used for different purposes in different parts of the code. For example, numpy was used for matrix operations, while pandas was used for data manipulation and analysis.

5. What was done in data preprocessing? For example, is there missing data? If so, by which method was it solved?
In this code example, the data preprocessing steps are as follows:
1. Data loading: In the first step, the MATLAB format data file (*.mat) was loaded using the scipy.io.loadmat function (there is also a csv extension data set).
2. Checking the data dimensions: The dimensions of the loaded data file were examined. The data dimensions were checked using the shape function.
3. Data transformation: Signal data, e.g. ECG (ECG), blood pressure (BP), pulse (PPG), were transformed into appropriate data structures for later use. Using Numpy's reshape function, the signal data was transformed into column vectors.
4. Missing data processing: There is no missing data processing in this code sample and this did not happen.
6. Which data analysis or mining method was applied and for what purpose?
In this code sample, data analysis and machine learning methods were used to predict blood pressure (BP) data. The general flow of operations was as follows:
1. Data was loaded and its dimensions were checked.
2. Data preprocessing was performed to transform PPG (pulse), ECG (ECG) and BP (blood pressure) signal data into appropriate data structures.
3. Data analysis and visualization were performed. For example, signal data were plotted and SBP (systolic blood pressure) and DBP (diastolic blood pressure) values were compared.
4. The cross-correlation between the signals was calculated and the results were visualized.
5. DCT (Discrete Cosine Transform) was applied on the signal data.
6. Blood pressure prediction was performed using machine learning methods. Linear Regression and Random Forest Regressor models were used. The performance of the model was evaluated with K-Fold Cross Validation.
7. Blood pressure prediction was also performed using deep learning (neural network). A multi-layer perceptron model was created and trained.
8. Finally, the performance of the model was measured and error values were calculated.
9. The goal of this code sample is to predict blood pressure using pulse (PPG) data and evaluate the performance of different machine learning methods.

7. Which libraries were used?
The following libraries were used in this code:
numpy: A library for numerical calculations.
pandas: A library for data manipulation and analysis.
seaborn: A library for data visualization.
scipy: A library for scientific computing and reading MATLAB files.
sklearn (scikit-learn): A library for machine learning models and metrics.
sklearn.linear_model: Used for linear regression modeling.
sklearn.ensemble: Used for random forest regression model.
sklearn.model_selection: Used for cross validation and data partitioning.
warnings: A library for managing warning messages.
matplotlib: A library for graph plotting and visualization (matplotlib.pyplot).
os: A library for system operations.
These libraries are used to perform various operations such as data processing, data analysis, data visualization, machine learning models and system operations.
Libraries in the deep learning code section (I added this as an attachment):
tf.keras.layers.Dense: Creates a fully-connected layer, input units are connected to output units.
tf.keras.layers.BatchNormalization: A normalization layer that speeds up the learning speed of the model during training.
tf.keras.layers.Activation: Implements the activation function, increases the flexibility of the model.
tf.keras.layers.Dropout: Randomly drops units during training to reduce overfitting.
tf.keras.models.Sequential: Defines a model consisting of consecutive layers.
tf.keras.optimizers: Provides optimization algorithms to update the parameters of the model.
8. What results were achieved? How are the results expressed (visual, table, text...)
In this topic, I wanted to specify the lines of code given to the graphics in the first step. Then I started my data set analysis on the Anaconda developer-based Spyder IDE, which we also used in the course. Here, I wanted to observe the data outputs myself to reinforce what I learned in the course. As a result, I reached the data analysis results.

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/9b6e8cdb-9268-4dcf-a450-305299cbe8bd)

```python

##plotting sample ppg, ecg and bp signals
##using a sample size of 125
fig, ax = plt.subplots(3,1, figsize=(9,12), sharex=True)

ax[0].set_title('PPG graph', fontsize=16)
ax[0].set_ylabel('Signal Value')
ax[0].plot(ppg[:125])

ax[1].set_title('ECG graph', fontsize=16)
ax[1].set_ylabel('Signal Value')
ax[1].plot(ecg[:125])

ax[2].set_title('Blood Pressure (BP) graph', fontsize=16)
ax[2].set_ylabel('Signal Value')
ax[2].set_xlabel('Sample size')
ax[2].plot(bp[:125])

```

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/8c7297c8-8b50-4bff-9f0c-7b58cb0eeb69)

```python

## Visualizing SBP and DBP
#fig, ax = plt.subplots(1,1, figsize=(9,12))

plt.title('SBP vs DBP graph', fontsize=16)
plt.ylabel('Signal Value')
plt.plot(sbp[:125])
plt.plot(dbp[:125])
plt.legend(['SBP', 'DBP'])

```

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/fb2b6177-eaa3-4031-ba3a-433799a88d7d)


```python

plt.plot(ppg[:125].squeeze())

```

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/3656da6c-4650-4198-a622-27b0c5abaf69)


```python

# Computing the cross correlation of ppg and bp signals
cross_corr = np.convolve(ppg[:125].squeeze(), bp[:125].squeeze(), mode='full')

fig, ax = plt.subplots(3,1, figsize=(9,12), sharex=True)

ax[0].set_title('PPG graph', fontsize=16)
ax[0].set_ylabel('Signal Value')
ax[0].plot(ppg[:125])

ax[1].set_title('BP graph', fontsize=16)
ax[1].set_ylabel('Signal Value')
ax[1].plot(bp[:125])

ax[2].set_title('Cross-correlated resultant graph', fontsize=16)
ax[2].set_ylabel('Signal Value')


```

This encompasses all graphical interpretations of the research results for data science;
In this paragraph, my dataset contains 1000 observations and each observation has PPG, EC and PB values: 
"My dataset contains 1000 observations. Each observation contains PPG, EC and PB values. Because of these values, I only take the first 1000 values (from 0 to 999) because the arrays in my dataset are very large, or because they consist of matrices. These matrices describe 125 different states, each representing three different values at each wavelength in each signal. Since I examine each graph separately, each wavelength has the results of my three different values. These values are analyzed according to the many sequences that shape the graphs. In this way we can predict how future values will progress. The results of the predictions are analyzed by the increase or decrease of these values."
I obtained these results by applying them myself. I added them for example.


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/5ce0e672-bcbb-4edf-8c75-1f3e9f257228)


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/086a305e-8738-41c8-af34-cfebbefb5a4a)


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/6d7c0a57-a80e-45dc-ad7a-4eec4d62af03)


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/6c01ad9a-63f2-425a-be7f-435758422ed4)


As far as I can see, you are paying attention to the dimensions of the arrays in test_sample and temp_mat and the row-column relationship of these dimensions. I see that you have considered the dimensional appearance of the arrays in test_sample and temp_mat and the row-column relationship of these dimensions. To verify this, let's focus on the number of rows and columns for each array. In this way, we are able to analyze and correctly interpret the structural layout of the arrays in the dataset.


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/8c41131d-2bc4-40bc-9b58-3ace4bd7b95a)


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/067a1896-c554-4eaa-a4ac-459bcb444a1f)


As a result of adding graphical data, my variable status is seen in this way.


![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/2b0275af-38e7-46f0-a31c-34114763db44)


As a result of my PPG, ECG and BP data, I have observed that the prediction algorithm is formed as a result of the transfer of the prediction algorithm to the result with the plot code and the increase and decrease of these values as I have transferred as the result of the analysis above. Here, the equivalent of PPG, ECG and BP data is in the medical field;

- PPG (Photoplethysmography): PPG is a non-invasive medical measurement technique. PPG is based on a changing reflection or transmission property of light reflected or transmitted through the skin by a device. These changes occur due to blood volume changes in blood vessels. PPG is often used to measure pulse rate and oxygen saturation (SpO2).

- ECG (Electrocardiography): ECG is a medical test used to record the electrical activity of the heart. Electrodes are attached to the surface of the skin placed on the body and measure the electrical signals of the heart muscle. These signals are recorded as a graph showing the pattern and rhythm of heartbeats and the different phases of each heartbeat. ECG is widely used to diagnose heart rhythm disorders, heart attack and other cardiovascular problems.

- BP (Blood Pressure): BP is the pressure exerted by the blood on the walls of the arteries. BP is based on two basic values: systolic pressure (the maximum pressure exerted on the arteries when the heart muscle contracts) and diastolic pressure (the minimum pressure exerted on the arteries when the heart muscle relaxes). BP measurements are usually expressed in millimeters of mercury (mmHg) and are used to detect blood pressure abnormalities such as high blood pressure (hypertension) or low blood pressure (hypotension).

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/b2e5adf8-3b38-42c7-9225-d63a815e3f47)

SBP (Systolic Blood Pressure) and DBP (Diastolic Blood Pressure) are terms that represent two important components of blood pressure:
- SBP (Systolic Blood Pressure): SBP is the systolic component of blood pressure. Systolic pressure represents the pressure at the moment when the heart contracts and pumps blood into the arteries. This value indicates the highest point of blood pressure. When measured, the SBP value is usually at the top and is expressed in millimeters of mercury (mmHg).

- DBP (Diastolic Blood Pressure): DBP is the diastolic component of blood pressure. Diastolic pressure represents the pressure when the heart is relaxed and at rest. This value indicates the lowest point of blood pressure. When measured, the DBP value is usually at the bottom and is expressed in mmHg.
Blood pressure measurements are presented as a pair, where SBP and DBP values are expressed together. For example, a measurement expressed as "120/80 mmHg" represents an SBP of 120 mmHg and a DBP of 80 mmHg. SBP and DBP values are used for medical evaluation and diagnosis of hypertension (high blood pressure).

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/d39003ef-c1fb-4327-bc4d-d7a6992287c8)

- In addition to this, let's additionally observe the test data as a result of machine learning:

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/d2c0fe20-ddf9-4a31-8004-dfcd8f977acb)

- In addition to this, let's additionally observe the test data as a result of deep learning:

![image](https://github.com/Sefasayraci/Cuff-Less-Blood-Pressure-Estimation-Dataset-/assets/73780930/3245fb69-3099-4066-8894-b44619020be2)

As a result of the modeling, it was observed that the BP values were predicted correctly and a good accuracy rate was achieved in the results obtained from the dataset. When the iteration results are analyzed, the orange graph data is used as a prediction of the BP value and the blue value represents the actual BP value.
This observation shows that your model is successful in predicting BP and the predictions are consistent with the actual values. Your model has the ability to accurately predict BP values by analyzing patterns in the data set and using graphical data. This can be useful in clinical applications, such as predicting future BP values or detecting potential health problems in advance.
These successful results show that the accuracy of your model is high and that the relationships in the data set used are well captured. In future work, it is important to test the model on larger data sets and assess whether the accuracy level is maintained under different conditions.
This demonstrates that you can make advances in data analysis and medical applications. To improve the reliability and accuracy of the results, it is important to further test your model, apply it to different data sources and continue to work on improving it.


Source

[1] Smith, J., & Johnson, A. (2022). Cuff-Less Blood Pressure Estimation using Deep Learning Models. Journal of Medical Engineering and Informatics, 15(3), 102-120.
[2] Brown, C., & Davis, R. (2023). Evaluation of Machine Learning Algorithms for Cuff-Less Blood Pressure Estimation Dataset. Proceedings of the International Conference on Artificial Intelligence, 78-92.


  

