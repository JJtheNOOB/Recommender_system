## Alternating Least Square Method
- Works really well with sparsity of the sparse matrix
- It fills out the sparse part of the matrix with prediction ratings if those users were to watch them
- The predictions of the highest ratings would then be the recommendations that can be offered to the user

## Algorithm:
- Matrix Factorization
   - Factor a matrix __R__ (m * n) __the user movie matrix__ into 2 matrix U (m * k) and R (k * n)
   - Errorij =  completion term * cost function * regularization term
