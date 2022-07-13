# Homeless Clustering Summary 
For the better part of the decade Maricopa County has struggled with homelessness. From 2018 - 2022 unsheltered homelessness has seen an increase of around 92% and has seen a steady increase since 2014. (Arizona Government Magazine) The increased rate of homelessness across the county can lead to potential issues with crime, public health, transportation, and government financial burden. In a 2017 external report by the RAND Corporation, analysts found that in California the average homeless person receives around $38,416 worth of public services. (RAND) Additionally potential outbreaks with diseases such as STDs, hepatitis and more are amplified by homeless individuals due to a lack of public health services. Reports by the CDC show that various hepatitis outbreaks in California saw increased efficacy in areas with high rates of homelessness. (CDC) Further the safety and community risk homeless people present cannot be ignored, with most citizens having increased anxiety or nerves when near homeless people and communities.

The homeless issue described above, then brings forth the question, how can we better understand homeless behaviors to make policy decisions that positively impact homeless populations. However, to build such a model, we first need an in depth understanding and awareness of homeless populations. So, to increase homeless data understanding and awareness, I propose the use of various statistical methods and techniques on homeless service data in the Maricopa County from 2014 to 2018.

From the use of various clustering algorithms, I was able to find that it is possible to cluster homeless people based on the number of services they use into 5 optimally chosen distinct clusters, ranked from "Very Low Usage" to "Very High Usage". After creating the final cluster model using Jenks Natural Breaks Optimization, I analyzed the final cluster and found that around 80% of homeless individuals fall into the "Very Low Usage" cluster, with the remaining 20% falling into the higher "Usage" clusters. Additionally, I was able to find various descriptive statistics regarding the most used services and plotted various statistical relationships.

Based on the clusters it becomes apparent that there's a high imbalance between the number of services provided and the number of homeless individuals utilizing them. We find that the median total count of services utilized for a homeless individual in our dataset from 2014 - 2018 comes out to only 2 services, while the max sits at around 685 services. Further the most occurred total service counts are 1, 2, 3, 4 & 5 accounting for 71% of the total services used. This shows that most individuals within Maricopa County are not taking full advantage of the services provided, leading to potential waste of resources. From this I suggest that more data will be needed to get a better idea of who and why services are not utilized. Ideally demographic data would greatly enhance our understanding. 

## Final Visualizations

### Vizualizing Jenks Natrual Breaks Optimization 
<img width="500" alt="Screen Shot 2022-07-13 at 7 26 51 AM" src="https://user-images.githubusercontent.com/88412646/178794274-67b8e63f-07c9-4768-ba78-4a0384236818.png">

On this graph we can see the clear Breaks/Usage Clusters that our model detected. The results are very fascinating and the graph clearly shows that clusters do exist based of the amount of services that homeless people use in the Maricopa County. Additionally it becomes clear that there is severe imbalance in the amount of services used as the majority of homeless individuals are not making use of services and fall with the low usage towards the far left.

### Bar Chart Cluster Distribution
<img width="500" alt="Screen Shot 2022-07-13 at 7 29 57 AM" src="https://user-images.githubusercontent.com/88412646/178794847-54c9b189-58cb-4bf8-ac8e-a804beceebe1.png">

This graph builds off our model and graphs the distribution of each cluster we found. It is clear that the majority of homeless indviduals fall within the 'Very Low Use' cluster. This shows a clear imbalance between service users in the homeless community. Though it is out of scope for this project, it's clear that there are other factors involved that may lead to this. For example it may be due to a lack of services in certain regions, improper resource management, or other external factors.

### Elbow Method for Optimal K Clusters 
<img width="500" alt="Screen Shot 2022-06-29 at 8 11 31 AM" src="https://user-images.githubusercontent.com/88412646/176506581-1b5f9bdb-777b-4f67-9711-e2fff4b92c30.png">

This graph shows the elbow method, which we used to choose the final number of clusters for our model. This method iterates through multiple versions of a model and tries to find the model that minimizes the amount of variation within clusters while maximizing variation between clusters. We then choose the optimal number of clusters based on the lowest number of clusters that min's the most variation.


### Final Evaluation Methods for Clusters
<img width="500" alt="Screen Shot 2022-06-29 at 8 01 39 AM" src="https://user-images.githubusercontent.com/88412646/176504982-f1bfba89-1341-4ff2-8d0d-d76dad3b1894.png">

## Exploratory Visualizations

### Initial Principal Component Analysis, with K Means Clusters for the various changes in color (code in prototype file)

Each of these graphs were used in the preliminary analysis and display a 'Projection' of the total dataset onto a scatterplot. As you can see the results of our projections are very hard to interpret and do not show any clear clusters within our dataset. Becuase of this we did not use these methods and instead used the model mentioned above. 

<img width="1100" alt="Screen Shot 2022-06-29 at 8 15 33 AM" src="https://user-images.githubusercontent.com/88412646/176507285-90327ed6-c66f-4467-a15b-cb90d7839742.png">

### Initial Principal Component Analysis, with DBSCAN for the various changes in color (code in prototype file)
<img width="1100" alt="Screen Shot 2022-06-29 at 8 16 38 AM" src="https://user-images.githubusercontent.com/88412646/176507482-6d0c22ea-417f-448a-bdf9-338a6ca612d5.png">

### Initial Principal Component Analysis, with BIRCH for the various changes in color (code in prototype file)
<img width="1100" alt="Screen Shot 2022-06-29 at 8 17 52 AM" src="https://user-images.githubusercontent.com/88412646/176507703-7f64a3db-be0a-4caa-a2f7-bba0a168c338.png">
