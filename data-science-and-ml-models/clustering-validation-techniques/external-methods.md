# External methods

Given a ground truth T, we want to derive Q(C,T) isthe quality measure for a cluster C

Q(C,T) is considered good if&#x20;

* The cluster is homogeneous - The purer the cluster the better
* Cluster is complete - Assign objects belonging to the same category in the ground truth to the same cluster
* Putting a Heterogeneous object into a pure cluster should be penalized more than putting it into a rag bag(miscellaneous cluster)
* Smaller clusters are preserved - splitting a small category into pieces is more harmful than splitting a large category into pieces

#### Commonly used External Measures

* Matching based measures - Purity, maximum matching, F-measure
* Entropy Based Measures - Conditional entropy, Normalized Mutual information, Variation of information
* Pairwise measures - TP, FN, FP, TN, Jaccard coefficiet, Rand Statistic, Fowlkes - Mallow

####

