# Facebook-Friend-Recommendation

Data soruce-https://www.kaggle.com/c/FacebookRecruiting

**1-Problem statement**
  - Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)

**2-Data Overview**
  - data contains two columns source and destination each edge in graph 
    - Data columns (total 2 columns):  
    - source_node         int64  
    - destination_node    int64  
 
**3-Business Objective and constraints**
  - No low-latency requirement.
  - Probability of prediction is useful to recommend ighest probability links

**4-Mapping given problem into supervised Learning Problem**
  -Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank,      katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.
 
**5-Performance Metric**
  - Both precision and recall is important so F1 score is good choice
  - Confusion matrix
