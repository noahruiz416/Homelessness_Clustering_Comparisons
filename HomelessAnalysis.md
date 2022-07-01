# Homeless Clustering Summary 
For the better part of the decade Maricopa County has struggled with homelessness. From 2018 - 2022 unsheltered homelessness has seen an increase of around 92% and has seen a steady increase since 2014. (Arizona Government Magazine) The increased rate of homelessness across the county can lead to potential issues with crime, public health, transportation, and government financial burden. In a 2017 external report by the RAND Corporation, analysts found that in California the average homeless person receives around $38,416 worth of public services. (RAND) Additionally potential outbreaks with diseases such as STDs, hepatitis and more are amplified by homeless individuals due to a lack of public health services. Reports by the CDC show that various hepatitis outbreaks in California saw increased efficacy in areas with high rates of homelessness. (CDC) Further the safety and community risk homeless people present cannot be ignored, with most citizens having increased anxiety or nerves when near homeless people and communities.

The homeless issue described above, then brings forth the question, how can we better understand homeless behaviors to make policy decisions that positively impact homeless populations. However, to build such a model, we first need an in depth understanding and awareness of homeless populations. So, to increase homeless data understanding and awareness, I propose the use of various statistical methods and techniques on homeless service data in the Maricopa County from 2014 to 2018.

From the use of various clustering algorithms, I was able to find that it is possible to cluster homeless people based on the number of services they use into 5 optimally chosen distinct clusters, ranked from "Very Low Usage" to "Very High Usage". After creating the final cluster model using Jenks Natural Breaks Optimization, I analyzed the final cluster and found that around 80% of homeless individuals fall into the "Very Low Usage" cluster, with the remaining 20% falling into the higher "Usage" clusters. Additionally, I was able to find various descriptive statistics regarding the most used services and plotted various statistical relationships.

Based on the clusters it becomes apparent that there's a high imbalance between the number of services provided and the number of homeless individuals utilizing them. We find that the median total count of services utilized for a homeless individual in our dataset from 2014 - 2018 comes out to only 2 services, while the max sits at around 685 services. Further the most occurred total service counts are 1, 2, 3, 4 & 5 accounting for 71% of the total services used. This shows that most individuals within Maricopa County are not taking full advantage of the services provided, leading to potential waste of resources. From this I suggest that more data will be needed to get a better idea of who and why services are not utilized. Ideally demographic data would greatly enhance our understanding. 

## Final Visualizations

### Vizualizing Jenks Natrual Breaks Optimization 
<img width="500" alt="Screen Shot 2022-06-29 at 8 02 32 AM" src="https://user-images.githubusercontent.com/88412646/176505118-4ce53d88-1687-4a8d-aa78-f90fac2ab96d.png">

### Bar Chart of Most Used Services 
<img width="500" alt="Screen Shot 2022-06-29 at 8 07 40 AM" src="https://user-images.githubusercontent.com/88412646/176505977-10c83e92-acf8-4269-8bb0-bbe3b9587a44.png">

### Scatterplots Showing Linear Relationships between various servies and total usage 
<img width="500" alt="Screen Shot 2022-06-29 at 8 09 48 AM" src="https://user-images.githubusercontent.com/88412646/176506296-8b3ce93b-9d19-48e1-9a15-a86b98db706e.png">

<img width="500" alt="Screen Shot 2022-06-29 at 8 10 15 AM" src="https://user-images.githubusercontent.com/88412646/176506357-a4d1cda2-57db-4b3d-b9ac-1512632ab121.png">

### Elbow Method for Optimal K Clusters 
<img width="500" alt="Screen Shot 2022-06-29 at 8 11 31 AM" src="https://user-images.githubusercontent.com/88412646/176506581-1b5f9bdb-777b-4f67-9711-e2fff4b92c30.png">

### Final Evaluation Methods for Clusters
<img width="500" alt="Screen Shot 2022-06-29 at 8 01 39 AM" src="https://user-images.githubusercontent.com/88412646/176504982-f1bfba89-1341-4ff2-8d0d-d76dad3b1894.png">

## Exploratory Visualizations

### Initial Principal Component Analysis, with K Means Clusters for the various changes in color (code in prototype file)
<img width="1100" alt="Screen Shot 2022-06-29 at 8 15 33 AM" src="https://user-images.githubusercontent.com/88412646/176507285-90327ed6-c66f-4467-a15b-cb90d7839742.png">

### Initial Principal Component Analysis, with DBSCAN for the various changes in color (code in prototype file)
<img width="1100" alt="Screen Shot 2022-06-29 at 8 16 38 AM" src="https://user-images.githubusercontent.com/88412646/176507482-6d0c22ea-417f-448a-bdf9-338a6ca612d5.png">

### Initial Principal Component Analysis, with BIRCH for the various changes in color (code in prototype file)
<img width="1100" alt="Screen Shot 2022-06-29 at 8 17 52 AM" src="https://user-images.githubusercontent.com/88412646/176507703-7f64a3db-be0a-4caa-a2f7-bba0a168c338.png">
