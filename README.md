# ISOMAP --- A dimensionality reduction method for nonlinear data points
Given 𝑚 data points, {𝑥1, x1,… xm} ∈ 𝑅, reduce the data to k dimensional
(1) Determine the neighbors of each data point
(2) Build a weighted graph A with nearest neighbors
(3) Compute pairwise shortest distance matrix D with distance functions
(4) Compute centering matrix H = I - 1/m*I_row*I_row.T, where I ∈ 𝑅m×m with all elements equal to zero, except for the k-th diagonal, whose values equal to one. I_row ∈ 𝑅m×1 with all elements equal to one.
(5) Compute matrix 𝐶 = −1/2*𝐻(𝐷ij^2)𝐻 ∈ 𝑅m×m
(6) Compute leading eigenvectors w1, w2,..., and eigenvalues 𝜆1, 𝜆2,..., of C
