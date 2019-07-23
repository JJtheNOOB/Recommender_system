## Alternating Least Square Method
- Works really well with sparsity of the sparse matrix
- It fills out the sparse part of the matrix with prediction ratings if those users were to watch them
- The predictions of the highest ratings would then be the recommendations that can be offered to the user

## Algorithm:
- Matrix Factorization
   - Factor a matrix __R__ (m * n) __the user movie matrix__ into 2 matrix __U__ (m * k) and __R__ (k * n)
   - Error_ij_ =  completion term * cost function * regularization term
   - Fill U and P with random values first, calculating error term based on the cost function
   - Then alternating back and forth between matrix U and matrix P to iteratively decrease the error
   - It continues of doing this until error term is minimized
   - Then U and P are multiplied together to the original matrix R
