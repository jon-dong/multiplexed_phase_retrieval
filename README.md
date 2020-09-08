# Multiplexed phase retrieval

How to solve multiplexed phase retrieval using a spectral method

## Definition

**Phase retrieval:** Find x in the equation:
```
y = |A x|^2
```
Many different algorithms have been proposed to solve this non-linear equation. 

**Multiplexed phase retrieval:** Find x_1, ..., x_k in the equation:
```
y = w_1 |A x_1|^2 + ... + w_k |A x_k|^2
```
In this more complex variant of phase retrieval, we are looking for several unknowns from multiplexed measurements. We assume the w_1, ..., w_k to be pairwise-different. 

## Spectral method

We will use a spectral method to solve multiplexed phase retrieval. Assuming A to be an i.d.d. random matrix, we define the following matrix:
```
Z = A^* diag(y) A^T
```
and retrieve x_1, ..., x_k as the k leading eigenvectors of Z. 

## Reference

More details in:
> Dong, J., Krzakala, F., & Gigan, S. (2019, May). Spectral method for multiplexed phase retrieval and application in optical imaging in complex media. In ICASSP 2019-2019 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP) (pp. 4963-4967). IEEE. Available at https://arxiv.org/abs/1810.13038
