# Optimized Permutation Testing

Code to accompany the paper "Optimized Permutation Testing for Information Theoretic Measures of Multi-Gene Interactions" by Kunert-Graf, Sakhanenko and Galas.

This consists of the following self-contained jupyter notebooks:

### plot_computational_complexity
This notebook generates synthetic SNP/phenotype data and times both the naive
permutation method and our method, over two different parameter ranges: first,
varying the number of individuals, and then varying the number of permutations.
It then plots the computation time of each approach (cf. Figure 1 of the main text).

### plot_transformed_distributions
This notebook first generates synthetic SNP/phenotype data for M individuals,
and creates a total of N permuted count tables using two methods: naive permutation,
and our method of transforming the count tables directly by iterative sampling of
the hypergeometric distribution. It then plots the distributions of count table
elements c_ij0 (cf. Figure 2 of the main text), and computes and plots the
associated multi-informations (cf. Figure 3 of the main text).

### plot_qq
This notebook generates permuted count tables using both the naive method and
our method, as in both notebooks above. It then performs a 2-sample Epps Singleton
test comparing the distributions of the count table entries. It does so over a range
of randomly-selected allele frequencies/phenotype frequencies. It then plots the
results (cf. Figure 4 of the main text).
