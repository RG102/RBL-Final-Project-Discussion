# Research Based Learning-Final-Project
FI2151 Modeling, Data Generator And Analysis

Multivariable Regression to Predict Housing Price in South Jakarta Region

List of Member :

1. 10223037 - Dietrich Pepalem Tarigan

2. 10223064 - Muhammad Rasyid Ghifari

3. 10223067 - Gwen Sevilen

4. 10223075 - Muhammad Syamsuddiin

Youtube Link For Presentation Video : https://youtu.be/LdDwt02ciOU

Notebook Gist : https://gist.github.com/RG102/7658470105ec36cc2ca0609ba2730e02

Presentation Slide : https://osf.io/num5c 

# *Multivariable Regression to Predict Housing Price in South Jakarta Region**

# 1. Abstract
This study aims to predict house prices based on key features such as land area (LT), building area (LB), number of bedrooms (JKT), and number of bathrooms (JKM). By analyzing data from South Jakarta properties, the work addresses data anomalies, such as negative prices, and uses feature normalization and logarithmic transformation for preprocessing. A linear regression model was developed and evaluated with metrics like MSE and R². Results show that LT and LB have the strongest correlation with house prices, with limitations in generalization due to data noise and outliers.

# 2. Background
The goal of this project is to build a predictive model for house prices using South Jakarta property data. Real estate pricing is influenced by features like location, size, and amenities. Existing methods often rely on robust regression techniques, yet many suffer from data irregularities. Key challenges include handling outliers, skewed distributions, and ensuring model interpretability. This work uses linear regression due to its simplicity and explanatory power, comparing feature importance to validate assumptions.

# 3. Method
Process Flow
Data Collection: Imported South Jakarta property dataset from Excel file.
Exploratory Data Analysis (EDA): Histograms, KDE plots, correlation matrix, and boxplots for identifying outliers and trends.
Preprocessing:
Removed outliers using the IQR method.
Applied feature normalization (MinMaxScaler) and logarithmic transformation on both features and target.
Modeling: Built a linear regression model using the LinearRegression class from sklearn.
Tools & Libraries
Python Libraries: pandas, numpy, matplotlib, seaborn, sklearn.
Key Functions:
LinearRegression: for modeling.
MinMaxScaler: for feature scaling.
np.log1p: for log transformation.
# 4.Results and Dicussion
Results
Model Performance:

Mean Squared Error (MSE): 0.15
R-squared (R²): 0.72
Regression Equation:


Feature Importance:

Land Area (LT) and Building Area (LB) are the most influential predictors of house prices.
Discussion
The regression model effectively predicts house prices with reasonable accuracy (R² = 0.72). However, limitations exist due to data noise and outliers. The high skewness in LT and LB distributions required significant preprocessing, including outlier removal and log transformations. Negative price entries were flagged as erroneous and excluded.

Visualizations
Correlation Matrix: Showed strong positive correlations between LT, LB, and price.
Scatter Plots: Highlighted improved data spread after log transformation.
# 5. Conclusion
This study successfully developed a linear regression model to predict house prices in South Jakarta based on key features such as land area, building area, number of bedrooms, and number of bathrooms. Unlike prior works, our approach addressed data irregularities like outliers and skewed distributions using robust preprocessing techniques, including the IQR method for outlier removal and logarithmic transformation for feature normalization. The model achieved a reasonable R² score of 0.72, emphasizing the significant influence of land and building area on pricing.

Key Differentiators:

Data Preprocessing: This work prioritized addressing data anomalies, such as negative prices and skewed distributions, ensuring a cleaner dataset for modeling.
Feature Selection: The focus on interpreting the importance of features enhanced the model's explanatory power compared to black-box approaches.
Future Work:

Incorporating additional features, such as property location or market trends, could improve the model's predictive accuracy.
Employing advanced algorithms, such as decision trees or ensemble methods, could address non-linear relationships and improve robustness against noise.
Expanding the dataset to include broader geographical areas and more recent data could enhance generalizability.
This study lays a foundation for using interpretable machine learning models in real estate pricing while highlighting opportunities for improvement in predictive performance and scalability.

# 6. References
References
[1]. Greyhatguy007. (n.d.). Machine Learning Specialization Coursera [GitHub repository]. Retrieved from https://github.com/greyhatguy007/Machine-Learning-Specialization-Coursera

[2]. Wisnu Anggara. (n.d.). Daftar Harga Rumah [Kaggle dataset]. Retrieved from https://www.kaggle.com/datasets/wisnuanggara/daftar-harga-rumah

[3]. Bishop, C. M. (2006). Pattern Recognition and Machine Learning. Springer.
