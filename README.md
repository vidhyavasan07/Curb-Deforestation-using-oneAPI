# Tree-Recommender-system-using-oneAPI
# PROBLEM STATEMENT ![image](https://user-images.githubusercontent.com/72274851/218500470-ec078b99-0a50-4b06-a2df-c09e47ecc187.png)
Reducing Deforestation using oneAPI.

# WORKING [image](https://user-images.githubusercontent.com/72274851/218503394-b52dfcc9-0620-4f44-94f5-46a09a5cc970.png)

The Tree recomender system can be used to reduce deforestation and increase tree cover.It totally consists of three models. 
### ✅ Forest Detector

### ✅Soil and Temperature Detector

### ✅Tree recommender 

The forest detector model takes a satellite image as input and detects area with less or no tree cover.The latitude and longitude of the detected area is found using google earth API and then passed into the soil and temperature detector model which predicts the soil type and temperature of the area. Tree recommender model takes the predictions as input and predicts the type of tree that can be grown in that area efficiently. 
All of the above mentioned models are built using oneDAL library.

# RESULTS![image](https://user-images.githubusercontent.com/72274851/218502434-f6e66043-0db0-4f85-b7f4-f33b2d33df1f.png)




# BUILDING THE MODEL![image](https://user-images.githubusercontent.com/72274851/218499685-e8d445fc-e35e-4ab5-abc1-c32462592603.png)


![image](https://user-images.githubusercontent.com/72274851/220130227-3c48e87b-3e68-4f1c-b0e4-8e3ad9a4805a.png)

✅Collecting data and preprocessing: collecting data was a very challenging as there was not enough data available on soil types and temperature.We had to create our own dataset.We used the oneAPI Data Analytics laibrary to for preprocessing the data. oneDAL library was highly useful in scaling,normalising etc.Using oneDAL library we were also able to decrease the training time.

✅Datasets used:
## ✅ Forest Detector-Deep Globe dataset fromkaggle

## ✅Soil and Temperature Detector-created our own datset

## ✅Tree recommender -created our own dataset


✅Models used to train the dataset:
## ✅ Forest Detector- Convolutional neural network

## ✅Soil and Temperature Detector- Decision Tree Regressor,Decision Tree classifier

## ✅Tree recommender- Ridge Regressor(oneDAL library)



✅Machine Learning: I likely learned about different machine learning algorithms and how they can be applied to predict crop yields and make recommendations for farmers.

✅Data Analysis: I likely gained experience in collecting and analyzing large amounts of data, including historical crop yield data and soil data, to train our machine learning models.

✅Agricultural Trends: I likely gained insight into current trends in agriculture and the challenges facing farmers, such as the need for sustainable and efficient crop production.

✅Collaboration: Building a project like this likely required collaboration with a team of experts in various fields, such as soil science, machine learning, and data analysis, and I likely learned the importance of working together to achieve common goals.

These are just a few examples of the knowledge and skills that i likely gained while building this project. 
Overall, building a crop recommendation application is a challenging and rewarding experience that requires a combination of technical expertise and agricultural knowledge.



