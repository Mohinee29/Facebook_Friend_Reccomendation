# Facebook_Friend_Reccomendation

<h2>Problem statement:</h2>

Given a directed social graph, have to predict missing links to recommend users (Link Prediction in graph)

<h2>Data Overview:</h2>

Taken data from facebook's recruting challenge on kaggle https://www.kaggle.com/c/FacebookRecruiting 
data contains two columns source and destination  edge in graph

Data columns (total 2 columns):
source_node int64
destination_node int64

<h2>Mapping the problem into supervised learning problem:</h2>

Generated training samples of good and bad links from given directed graph and for each link got some features like no of followers, is he followed back, page rank, katz score, adar index, some svd fetures of adj matrix, some weight features etc. and trained ml model based on these features to predict link.

<h2>Business objectives and constraints:</h2>

No low-latency requirement. Probability of prediction is useful to recommend ighest probability links.

<h2>Performance metric for supervised learning:</h2>

Both precision and recall is important so F1 score is good choice Confusion matrix.

<h2>CREDITS: APPLIED AI COURSE</h2>
