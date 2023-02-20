# Cryptocurrencies

## Purpose

The intention is to create a report that shows the cryptocurrencies trading market in order to group them in a classification system for this new investments.For this analysis we'll use unsupervised learning to process and cluster data. Additionally, reduce its dimensions and principal components using PCA. The data will be processed to fit the machine learning models. Visuallizations will be presented to share the findings with the board.


## Results

- Preprocessing the Data for PCA

The firt transformation was to keep all crypos being traded. 

![image](https://user-images.githubusercontent.com/114015620/220173606-e0329caa-2348-46db-b98a-8c6cc4a3c420.png)

Then only the coins that were mined.

![image](https://user-images.githubusercontent.com/114015620/220173750-52fe3b4e-eac8-41bd-bf71-b22eebc461d5.png)

No coin name column since it will not be used in the algorithm. 

![image](https://user-images.githubusercontent.com/114015620/220173915-33e56120-8244-442b-a98a-dd890fd1e00c.png)

Then, remove strings with the get_dummies function. 

![image](https://user-images.githubusercontent.com/114015620/220174272-ddc90b71-52ea-42d7-a585-0146473b41ea.png)

For this step it was finally used StandardScaler() to tranform it

![image](https://user-images.githubusercontent.com/114015620/220174385-ab93b6fe-4ab7-4881-8b49-c4c946ff6b7d.png)

- Reducing Data Dimensions Using PCA

By using PCA, data was transformed into thre principals (P1, P2, P3=

![image](https://user-images.githubusercontent.com/114015620/220174530-5e00d072-088e-4cbc-82fb-ea83a7d16e47.png)


- Clustering Cryptocurrencies Using K-means

An Elbow curve was performed on the data to estime the k value fo KMeans Model.

[ELBOW]

The model ran with k=4, as seen in the curve. 

![image](https://user-images.githubusercontent.com/114015620/220174831-b2213f24-118c-4a8b-be26-120c35673ea0.png)

Both data frames, were merged.

![image](https://user-images.githubusercontent.com/114015620/220175093-562c1273-385d-4f48-a4c7-6249f0edd002.png)

The fnal DataFrame looks as follows 

![image](https://user-images.githubusercontent.com/114015620/220175230-aeb26992-0fa6-4b52-a901-3ff78d4d7aa8.png)

Includig predicted values, coin names and classes. 


- Visualizing Cryptocurrencies Results

Visuallly a 3D-Scatter is presented with PCA and cluster data.

[3D-Scatter]

Below a table is shown

[table]

After all the transformations and machine learning models we can say that 

![image](https://user-images.githubusercontent.com/114015620/220175578-9067e034-a448-47ea-82ac-fa939a3e8948.png)

Data used Scaler transformation to be prepared for Scatter plot TotalCoinSupply and TotalCoinsMined.

[Scatter:new DataFrame with the scaled data in XX and the index of the original DataFrame]

Resulting in the DataFrame

![image](https://user-images.githubusercontent.com/114015620/220175919-2089f169-e194-4732-a063-3c741afa71f4.png)

Resulting in the

[hvplot.scatter plot using x="TotalCoinsMined" and y="TotalCoinSupply".]


## Summary
