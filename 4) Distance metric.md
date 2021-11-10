https://medium.com/@kunal_gohrani/different-types-of-distance-metrics-used-in-machine-learning-e9928c5e26c7

https://iq.opengenus.org/euclidean-vs-manhattan-vs-chebyshev-distance/

https://chris3606.github.io/GoRogue/articles/grid_components/measuring-distance.html

##### Minkowski distance - Lp norm

##### Manhattan distance - L1 norm 
-  city block distance, or taxicab geometry if we need to calculate the distance between two data points in a grid-like path. Manhattan distance metric can be understood with the help of a simple example.
- think of real world roads (we have grids, so cant really have euclidean distance) (path from my hostel to mess)
- “On the Surprising Behavior of Distance Metrics in High Dimensional Space”, by Charu C. Aggarwal, Alexander Hinneburg, and Daniel A. Kiem. “ for a given problem with a fixed (high) value of the dimensionality d, it may be preferable to use lower values of p. This means that the L1 distance metric (Manhattan Distance metric) is the most preferable for high dimensional applications.”
- Thus, Manhattan Distance is preferred over the Euclidean distance metric as the dimension of the data increases. This occurs due to something known as the ‘curse of dimensionality’.

##### Euclidean distance - L2 norm
Euclidean distance is the straight line distance between 2 data points in a plane.
##### Chebyshev distance - L-inf norm

###### from manhattan to chebyshev, consider the all the points from origin of 1 unit distance. Manhattan has the least number of points and chebyshev has the highest.  (rombus to squr)


![alt text](https://github.com/shailymishra/Machine-Learning-Concepts/images/jDlvI.png)


##### Hamming distance 
- Hamming distance is a metric for comparing two binary data strings. While comparing two binary strings of equal length, Hamming distance is the number of bit positions in which the two bits are different.
The Hamming distance between two strings, a and b is denoted as d(a,b).
In order to calculate the Hamming distance between two strings, and, we perform their XOR operation, (a⊕ b), and then count the total number of 1s in the resultant string.
Suppose there are two strings 11011001 and 10011101.
11011001 ⊕ 10011101 = 01000100. Since, this contains two 1s, the Hamming distance, d(11011001, 10011101) = 2.


##### Cosine distance
- Cosine distance & Cosine Similarity metric is mainly used to find similarities between two data points. As the cosine distance between the data points increases, the cosine similarity, or the amount of similarity decreases, and vice versa. Thus, Points closer to each other are more similar than points that are far away from each other. Cosine similarity is given by Cos θ, and cosine distance is 1- Cos θ. Example:-

- Cosine metric is mainly used in Collaborative Filtering based recommendation systems to offer future recommendations to users.
Taking the example of a movie recommendation system, Suppose one user (User #1) has watched movies like The Fault in our Stars, and The Notebook, which are of romantic genres, and another user (User #2) has watched movies like The Proposal, and Notting Hill, which are also of romantic genres. So the recommendation system will use this data to recommend User #1 to see The Proposal, and Notting Hill as User #1 and User #2 both prefer the romantic genre and its likely that User #1 will like to watch another romantic genre movie and not a horror one.
Similarly, Suppose User #1 loves to watch movies based on horror, and User #2 loves the romance genre. In this case, User #2 won’t be suggested to watch a horror movie as there is no similarity between the romantic genre and the horror genre.
Conclusion
In this blog post, we read about the various distance metrics used in Machine Learning models. We studied about Minkowski, Euclidean, Manhattan, Hamming, and Cosine distance metrics and their use cases.
Manhattan distance is usually preferred over the more common Euclidean distance when there is high dimensionality in the data. Hamming distance is used to measure the distance between categorical variables, and the Cosine distance metric is mainly used to find the amount of similarity between two data points.

##### Chess

In chess, all the three distances are used as follows:

the distance between squares on the chessboard for rooks is measured in Manhattan distance
kings and queens use Chebyshev distance
bishops use the Manhattan distance (between squares of the same color) on the chessboard rotated 45 degrees, i.e., with its diagonals as coordinate axes.
To reach from one square to another, only kings require the number of moves equal to the distance (euclidean distance) rooks, queens and bishops require one or two moves



##### Matrix distance metric