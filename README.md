# Tree-Recommender-system-using-oneAPI
# PROBLEM STATEMENT 
Reducing Deforestation using oneAPI.

# WORKING

The Tree recomender system can be used to reduce deforestation and increase tree cover.It totally consists of three models. 

 ✅ Forest Detector

 ✅Soil and Temperature Detector

 ✅Tree recommender 

The forest detector model takes a satellite image as input and detects area with less or no tree cover.The latitude and longitude of the detected area is found using google earth API and then passed into the soil and temperature detector model which predicts the soil type and temperature of the area. Tree recommender model takes the predictions as input and predicts the type of tree that can be grown in that area efficiently. 
All of the above mentioned models are built using oneDAL,oneDNN libraries.


# BUILDING THE MODEL


![image](https://user-images.githubusercontent.com/72274851/220130227-3c48e87b-3e68-4f1c-b0e4-8e3ad9a4805a.png)

✅Collecting data and preprocessing: collecting data was very challenging as there was not enough datasets available on soil types and temperature.We had to create our own dataset.We used the oneAPI Data Analytics laibrary to for preprocessing the data. oneDAL library was highly useful in scaling,normalising etc.Using oneDAL library we were also able to decrease the training time.
✅satellite images used for training forest detector is taken from deepglobe classification 
        https://www.kaggle.com/datasets/balraj98/deepglobe-land-cover-classification-dataset

✅Datasets used:

      ✅ Forest Detector-Deep Globe dataset from kaggle

      ✅Soil and Temperature Detector-created our own datset

      ✅Tree recommender -created our own dataset


✅Models used to train the dataset and their respective ml/dl algorithms:

      ✅ Forest Detector- Convolutional neural network

      ✅Soil and Temperature Detector- Decision Tree Regressor,Decision Tree classifier

      ✅Tree recommender- Ridge Regressor(oneDAL library)

✅Testing and Decision making -After the models were trained they were tested and produced a medium accuracy.The predictions can be used to effectively increase tree cover and reduce climate change,air pollution etc.

# RESULTS

# ✅Classification made by Forest detector-

![Screenshot 2023-04-08 193215](https://user-images.githubusercontent.com/102335494/230726084-4aa18344-2719-4666-918f-6c2db7c157d6.png)

![resnet](https://user-images.githubusercontent.com/102335494/230726152-d133f448-d364-451d-8598-5abb245ca5ea.png)

![image](https://user-images.githubusercontent.com/102335494/230726356-0d280d4d-189d-4898-a314-8591c5811360.png)

![inceptionv3](https://user-images.githubusercontent.com/102335494/230726125-7f9d06b5-2364-4612-977b-9f4efc17279a.png)


# ✅Prediction made by Soil-Temperature Detector

![soil_detection_output](https://user-images.githubusercontent.com/102335494/230724614-0d3d32d7-7f5f-4711-8c86-d18b0f8e3367.png)



# ✅Prediction made by Soil-Temperature Detector

![tree_output](https://user-images.githubusercontent.com/102335494/230724638-29f024fe-b679-48b0-883e-0c72519aa241.png)




# Why oneAPI is Preferred

![graph](https://user-images.githubusercontent.com/102335494/230723887-cd67b089-3ac1-466a-a025-27a3417284a8.png)


✅The models when tested using oneAPI took less time to train and test when compared to other platforms

✅Intel oneDNN library allows us to use multithreading.For CNN (forest detector),the multithreading model makes Training efficient for many number of layers and many    epochs for a huge datasets.
    Eg:config.intra_op_parallelism_threads = 56
    
✅daal4py can be used when we are dealing with large datasets or real time processing model.





# DevMesh

https://devmesh.intel.com/projects/curb-deforestation-using-intel-oneapi








