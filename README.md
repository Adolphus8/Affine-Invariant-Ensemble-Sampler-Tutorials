# Affine Invariant Ensemble Sampler Tutorials
This repository presents a collection of tutorials (written in MATLAB) which seeks to demonstrate the implementation of the Affine Invariant Ensemble Sampler based on the works by [Goodman and Weare (2010)](https://projecteuclid.org/euclid.camcos/1513731992). The associated literature is available in the "*References*" folder. Currently, 2 tutorials are being presented here aimed at allowing users who are new such sampler find their footing around its concept and its workings. To help facilitate the users in understanding the workings of the sampler as well as the objectives of the tutorials in a simplified manner, a summarised set of notes is also made availale in the "*References*" folder. The details to these tutorials are as follows:

## Tutorials:

### 1) Example Comparison:
This tutorial seeks to provide an illustration of the Affine-invariant property of this Ensemble sampler. 

In most instances, when one encounters a highly-anisotropic target distribution, one approach would be to perform an Affine transformation so as to simplify the form of the target distribution and allow for it to be sampled from easily. From there, an inverse Afffine transformation is performed on the generated samples so as to obtain the associated samples that is obtained indirectly from the original highly-anisotropic target distribution. 

For an Affine-invariant sampler, such as the Ensemble sampler here, it is able to sample directly from both the highly-anisotropic and the Affine-transformed distributions and views both distributions as equal. What this means is that an Affine-invariant sampler's sampling performances is unaffected regardless of whether that target distribution from which it is sampling is scaled or not. This tutorial aims to highlight this property of the Ensemble sampler and as a comparison, the [Metropolis-Hastings](https://doi.org/10.1093/biomet/57.1.97) sampler will also be implemented to demonstrate the latter's absence of the Affine-invariant property.

### 2) Example Rosenbrock:
This tutorial seeks to evaluate the robustness and strength of the Ensemble sampler in sampling from a highly-anisotropic distribution which cannot be re-scaled via Affine-transformation. As a comparison, the [Metropolis-Hastings](https://doi.org/10.1093/biomet/57.1.97) sampler will also be implemented to demonstrate the relative strength of the Ensemble sampler over the latter in samplign from such complex distributions.
