# Prediting Water Potability
Building a predictive model to determine whether or not the water is potable 

# Business Problem

Access to safe drinking water is essential to human health and well being. It is a basic human necessity and requirement of effective public health policy. However, access to clean water continues to be an issue at the regional, national and international levels. Research shows that investment in clean water supply and sanitation projects can yield a net economic benefit, as the reduction in adverse health effects and health care costs allow the population to flourish in economically beneficial roles. 

Countries such as Eritrea, Papua New Guinea and Uganda have the lowest access to clean water close to home, where almost 60% of the population lacks access to safe drinking water. Having the ability to identify unsafe drinking water for these residents has the potential to save countless lives.

By applying statistical models and machine learning techniques, we can help countries around the world test their water and provide access to clean water in their area. This will improve the health of the countries’ populations and lessen the burden of finding drinkable water, consequently leading to economic development. Our exploration can help identify important features of safe drinking water which will allow others to expand our research to additional populations. Expanding use of machine learning techniques to identify clean water can save lives around the world. 

# Modeling Ideas
Our problem is a supervised classification problem, where we will identify if the water is safe for human consumption or not. There are 9 features that we will explore to identify our target variable, potability (if the water is safe for consumption). A potability of one denotes drinkable water and a potability of zero denotes unsafe water. Our features includes: 
* pH of water: the acidity or basic of water (0 to 14)
* Hardness: capacity of water to precipitate soap in milligram per liter (mg/L)
* Solids: total dissolved solids in parts per million (ppm)
* Chloramines: Amount of Chloramines in parts per million (ppm)
* Sulfate: Amount of Sulfates dissolved in milligram per liter (mg/L)
* Conductivity: Electrical conductivity of water in microsiemens per centimeter (μS/c)
* Organic_carbon: Amount of organic carbon in parts per million (ppm)
* Trihalomethanes: Amount of Trihalomethanes in microgram per liter (μg/L)
* Turbidity: Measure of light emitting property of water in nephelometric turbidity units (NTU)

# Data Details
We obtained our data through Kaggle, an online community for data science competitions and datasets. The data contains water quality metrics for 3276 different water bodies. The data points are numerical for each of the features. We expect to convert pH of water into a categorical variable to improve our prediction model.

Through exploring the data we find that each feature is a float and the target variable is a binary variable. In the target variable, 1998 water bodies are not potable and 1278 water bodies are potable. The ratio is about 5:3 to the majority class. 

There are also some missing values in the data’s features which include:
* pH: 491 missing values
* Sulfate: 781 missing values
* Trihalomethanes: 162 missing values

We expect to fill the missing values with the mean, mode or median value of the feature. 
