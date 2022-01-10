# Prediction of the possibility to open a new station :

In this project we aim to predict the need to open a new bike station 
according to the realtime observations of the Vélib api https://www.velib-metropole.fr/donnees-open-data-gbfs-du-service-velib-metropole.

- Vélib' is a large-scale public bicycle sharing system in Paris, France. Launched on 15 July 2007, the system encompassed around 14,500 bicycles and
1,400 bicycle stations,located across Paris and in some surrounding municipalities, with an average daily ridership of 85,811 in 2011

Throughout the project we make use of Kibana as a streaming tool that streams data from Vélib api then Spark as a consumer for this api 
finally the predictions results are indexed into elasticsearch and visualized via Kibana .

![Sans titre](https://user-images.githubusercontent.com/75638904/148834277-672a5ee9-79c7-498b-b67e-e81484371b77.png)

The project is realized under the following steps : 
- Produce data from Vélib api using kafka producer 
- Develop machine learning alogorithm to prredic the possibility to open a new station (RandomForest)
- Consume the produced data by Spark Consumer 
- Index data to elasticsearch 
- Create dashboard using kibana 
