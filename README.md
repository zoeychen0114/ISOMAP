# ISOMAP --- A dimensionality reduction method for nonlinear data points
Given ð data points, {ð¥1, x1,â¦ xm} â ð, reduce the data to k dimensional
(1) Determine the neighbors of each data point
(2) Build a weighted graph A with nearest neighbors
(3) Compute pairwise shortest distance matrix D with distance functions
(4) Compute centering matrix H = I - 1/m*I_row*I_row.T, where I â ðmÃm with all elements equal to zero, except for the k-th diagonal, whose values equal to one. I_row â ðmÃ1 with all elements equal to one.
(5) Compute matrix ð¶ = â1/2*ð»(ð·ij^2)ð» â ðmÃm
(6) Compute leading eigenvectors w1, w2,..., and eigenvalues ð1, ð2,..., of C
