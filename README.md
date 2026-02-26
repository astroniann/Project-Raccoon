# Project-Raccoon

Eager vs Lazy Learning 
we use lazy learning with K-NN
k-Nearest Neighbor (k-NN)



THe stated reasons;

The Core Idea (Slide 17–18)
k-NN is the most famous lazy learner. The intuition is beautifully simple:
"Things that are similar to each other tend to belong to the same class."
If you want to classify a new point, find the k most similar training examples and let them "vote" on the class.
How it Works Step by Step:

Represent every data point as coordinates in space (one dimension per feature)
When a new point arrives, calculate its distance to every training point
Find the k closest training points (the "k nearest neighbors")
For classification: take a majority vote — whichever class appears most among the k neighbors wins
For regression (predicting a number): take the average value of the k neighbors

Distance Metric
The standard way to measure distance is Euclidean distance — the straight-line distance in n-dimensional space, just like the distance formula from geometry:
dist(X1, X2) = √[(x1₁-x1₂)² + (x2₁-x2₂)² + ...]
The Voronoi Diagram (Slide 18)
When you use k=1 (1-nearest neighbor), every point in space gets assigned to the class of whichever training point is closest to it. The boundaries between these regions form a Voronoi diagram — a beautiful geometric pattern showing exactly where the classifier switches from one class to another.
