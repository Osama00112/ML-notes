# K-Means Clustering

### K-Means
![image](https://user-images.githubusercontent.com/54764108/167300245-de36def3-67a9-4750-8f1d-c8383451c394.png)

Suppose we have a scattered  set of data points based on two variables. <br>
Can we identify certain groups in these data set? <br>
**K-Means** is a complex algorithm designed to find these groups.

* **Step 1:** Choose the number **K** of clusters
* **Step 2:** Select at random K points, the centroids(not necessarily from your dataset)
* **Step 3:** Assign each data point to the closest centroid => That forms K clusters
* **Step 4:** Compute and place the new centroid of each cluster
* **Step 5:** Reassign each data point to the new closest centroid. <br>
If any assignment took place, go to STEP 4, otherwise go to FIN.
* **FIN:** Model is ready.

### Example
<img src = https://user-images.githubusercontent.com/54764108/167300642-01e7356a-839f-4e9b-927f-79f3033e9b29.png width = "500" >

#### Step 1 : 
Let K = 2
#### Step 2 : Selecting random K = 2 points, the centroid
<img src = https://user-images.githubusercontent.com/54764108/167300721-7773cab1-c643-4ed1-8c8b-1be1ec90557f.png width = "500" >

#### Step 3 : Forming K = 2 clusters
<img src = https://user-images.githubusercontent.com/54764108/167300834-38d79cd9-ef55-4633-a9a2-ef6812eff625.png width = "400" > <img src = https://user-images.githubusercontent.com/54764108/167300819-18b4a8ef-c243-4ea9-a7d1-e9eefcd28283.png width = "400" >

#### Step 4 :
<img src = https://user-images.githubusercontent.com/54764108/167300963-f7b92282-b2ae-4995-9f40-faa1d48197b8.png  width = "400" > <img src = https://user-images.githubusercontent.com/54764108/167300982-e6b1f6a0-8f67-4cb4-87ea-d529627cb278.png  width = "400" > 

* We compute the center of gravity/mass of clusters and make new centroids and replace them with the old ones.

#### Step 5 : Reassignment
<img src = https://user-images.githubusercontent.com/54764108/167301119-df8464f4-d0d8-44f1-bd95-08503490dfeb.png  width = "400" > <img src = https://user-images.githubusercontent.com/54764108/167301137-6635f34f-c241-4080-ace2-3fc323a9861b.png  width = "400" > 

#### Repeating:
Iterative approaches until the algorithm converges to the final assignments.

<img src = https://user-images.githubusercontent.com/54764108/167301239-bf24313f-9558-4c40-8045-ce2f70afbf3f.png  width = "400" > <img src = https://user-images.githubusercontent.com/54764108/167301256-ab9ef2c3-3ca5-41d6-8a84-892fc01244f2.png  width = "400" > 

