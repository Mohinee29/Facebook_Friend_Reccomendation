# Facebook Friend Reccomendation

<h2>Problem statement:</h2>

Link Prediction in graph: Given a social graph, predict and recommend the missing links to users.

<h2>Data Overview:</h2>

Dataset is taken from Facebook's recruiting challenge on kaggle (https://www.kaggle.com/c/FacebookRecruiting), which is a directed graph having two attributes, source and destination edge in the graph

<h3>Database Attributes: </h3>
source_node (int64) and destination_node (int64)

<h2>Mapping the problem into supervised learning problem:</h2>

Training samples of good and bad links were generated from the given directed graph and for each link, features like number of followers, followedBack status, page rank, Katz score, Adar index, svd features for Adj. Matrix, weight features were extracted and ML model was trained on these features to predict the link.

<h2>Business objectives and constraints:</h2>

Low-latency requirement. Probability of prediction is useful to recommend highest probability links.

<h2>Performance metric for supervised learning:</h2>

Both precision and recall is important so F1 score is good choice, which was calculated using the Confusion matrix.

<h2>CREDITS: APPLIED AI COURSE</h2>
