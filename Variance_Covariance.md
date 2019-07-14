Difference between n and (n-1):

(n-1) is called the degrees of freedom and if we use n the estimator will be unbiased.

The population variance from a sample when the population mean is unknown, the uncorrected sample variance is the mean of the squares of deviations of sample values from the sample mean (i.e. using a multiplicative factor 1/n). In this case, the sample variance is a biased estimator of the population variance.
When Multiplying with the uncorrected sample variance by the factor n/(n-1) gives an unbiased estimator of the population variance.


Calculation of covariance matrix:

covariance matrix is simply set of variances and covariances between pairs of columns. A position of any element in the covariance matrix corresponds to variance/covariance between a pair of two columns. Each row of covariance matrix in the sample or population depending on which option, needs to be converted to a deviation score based on the aggregate data within each column. Then, we find the deviation score sums for each feature measured against all other features. The last step is to divide each element by either n - 1 if we're using a sample or N if we are using the entire population.

#properties of covariance matrix
Addition to constant vectors<br>

Let $a$ be a constant K1 vector and let x be a K1 random vector. Then,
$$Var[a + x] = Var[x]$$

Multiplication by constant matrices<br>

Let $b$ be a constant $M * K$ matrix and let x be a K*1 random vector. Then,
$$Var[bx] = bVar[x] b ^t$$

Linear transformations<br>

Let $a$ be a constant $M * 1$ vector, $b$ be a constant $M * K$ matrix and $x$ a Kx1 random vector. Then, combining the two properties above, one obtains
$$Var[a + bx] = bVar[x] b ^t$$

Symmetry<br>

The covariance matrix $Var[x]$ is a symmetric matrix, that is, it is equal to its transpose:<br>
$$Var[x] b ^t = E[(x - E[x])(x - E[x]^t)]^t$$<br>
$$= E[((x - E[x])(x - E[x]^t)^t]$$<br>
$$= E[(x - E[x])(x - E[x]^t)]$$<br>
$$= Var[x] $$
