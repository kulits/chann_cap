# `pickle` files

As an output of some of the scripts either `pkl` or `dill` files are saved to
be imported later on for costly calculations. These files are mainly the output
of `lambdify` functions from `sympy`, where an analytical result is turned into
a function that can be numerically evaluated using `numpy`.

The functions are not pushed to the `GitHub` repo given the large file size.
But these folder is added such that when interested users want to run the
notebooks that generate the files, these files can be directly exported to this
location.

The important files in this directory are:


- `two_state_moment_lambdify.dill`, `three_state_moment_lambdify.dill` :  These
  files, generated by the notebook
  `chemical_master_steady_state_moments_general.ipynb`, are `lambdify`
  functions generated with `sympy` that compute the numerical value of the
  moments of the mRNA and protein distribution given a set of rate parameters.
  Specifically the functions evaluate up to the **third protein moment**
  $\left\langle m^0 p^3 \right\rangle$ with all the necessary moments needed.
  These moments assume that both, the mRNA and the protein distribution reach
  steady state, and don't account for the gene copy number variation that cells
  go through as they replicate their genomes and divide.
    - NOTE : These particular functions had to be exported using the
      `cloudpickle` library rather than the usual `pickle` library for reasons
      I don't fully understand.

- `binom_coeff_matrix.pkl` : This file, exported by the notebook
  `binomial_moments.ipynb` contains a numerical matrix used to compute the
  moments of the mRNA and protein distribution right after a cell divided and
  each of the molecules underwent a binomial partitioning event.