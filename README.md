# Assignment-5
# Define matrices A and B
A <- matrix(1:100, nrow=10)
B <- matrix(1:1000, nrow=10)

# Attempt to compute the inverse of matrix A
if (det_A <- det(A)) {
  A_inv <- solve(A)
  cat("Inverse of matrix A:\n")
  print(A_inv)
} else {
  cat("Matrix A is singular, its determinant is zero.\n")
}

# Calculate the determinant of matrix B
if (is.square <- nrow(B) == ncol(B)) {
  det_B <- det(B)
  cat("\nDeterminant of matrix B:", det_B, "\n")
} else {
  cat("Matrix B is not square, its determinant cannot be calculated.\n")
}
Procedure:
Define Matrices: To begin, define A and B using the given values. R's matrix() function can be used to construct matrices.
Compute the Inverse of Matrix A: To compute the inverse of matrix A, use R's solution() function. To prevent mistakes, make sure the matrix is singular—that is, that its determinant is not zero—before computing the inverse.
Determine the Matrix B Determinant: It is not possible to compute B's determinant directly because it is not square. Therefore, before attempting to compute B's determinant, it is imperative to confirm that B is square.
Show Results: Lastly, display the determinant of B and the inverse of A results, together with any pertinent comments about the squareness or singularity of the matrices.
