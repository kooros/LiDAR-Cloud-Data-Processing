# LiDAR-Cloud-Data-Processing
by Kooros Moabber

## Visualize datasets
![Cloud before Ground Removal](Cloud.png)

# Task1: 
## Ground Plane Removal
### Histogram before ground removal
![Histogram before ground removal](Histogram_initial.png)

**Ground level for dataset 1= 61.99766250000003**

**Ground level for dataset 2= 61.981925**

### Histogram after ground removal
![Histogram after ground removal](Histogram_withoutground.png)

### Cloud after ground removal
![Cloud after ground removal](Cloud_withoutground.png)

# Task2:
## Optimal DBSCAN Clustering
### Clustered cloud with unoptimal eps
![Clustered_Cloud_without ground with_unoptimal_eps](Clustered_Cloud_withoutground_unoptimal_eps.png)

### Effect of eps and min samples on cluster number
![eps_and_min_samples_on_cluster_number](ClusterNo_eps_MinSample_Effect.png)

### Optimal eps by Elbow Point
![Optimal_eps_by_Elbow_Point](ElbowPoint.png)

**optimal_eps1 = 1.5** *# elbow point* 

**optimal_eps2 = 2** *# elbow point* 
### Clustered Cloud withoutground with optimal eps
![Clustered_Cloud_without ground_with optimal_eps](Clustered_Cloud_withoutground_optimal_eps.png)

# Task3:
## Find catenary by selecting the largest cluster
### Biggest span cluster data:
- dataset1 data (eps=1.5, min_sample=5): 
  - Cluster Label : 1
  - Cluster span: 115.583
  - min(x) of dataset1 : 26.498
  - max(x) : 62.140
  - min(y) : 80.019
  - max(y) : 159.960

- dataset2 data (eps=2, min_sample=5): 
  - Cluster Label : 7
  - Cluster span: 106.761
  - min(x) of dataset1 : 26.498
  - max(x) : 37.007
  - min(y) : 0.043
  - max(y) : 79.976
 
## plot of the catenary cluster 
![plot_of_the_catenary_cluster](Catenary_with_optimal_eps.png)
