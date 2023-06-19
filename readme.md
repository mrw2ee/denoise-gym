# Denoise Gym
Personal notes coming up to speed with current (Summer 2023) use of denoising algorithms in a broader plug-and-play framework for solving inverse problems. A fantastic starting point is the [Scientific Computational Imaging Code (SCICO)](https://github.com/lanl/scico) which is a well-curated collection of tools, tutorials, and pre-trained models. This repo contains notebooks and scripts as we dig a little deeper: extending demos, reproducing results, and referencing larger datasets.

# SCICO submodule
SCICO is currently under active development. While it can be installed via [pip](https://scico.readthedocs.io/en/stable/install.html#from-pypi), the pip version may lag the [github](https://scico.readthedocs.io/en/stable/install.html#from-github) version. For this reason, SCICO is included here as a [submodule](./scico_local/).  SCICO can then be manually using pip from `.\scico_local`.

```
cd scico_local
pip install -e .  # Installs SCICO from the current directory in editable mode
```

# Datasets
Many papers on denoising algorithms reference the so-called BSDS68 dataset. We could not find an authoritative definition ([see here](https://github.com/clausmichele/CBSD68-dataset)). However, it appears to be a subset of the [Berkeley Segmentation Data Set and Benchmarks 500 (BSDS500)](https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html). Specifically, a subset of the [validation images](./BSDS500/BSDS500/data/images/val).
 

# References
K. Zhang, W. Zuo, Y. Chen, D. Meng and L. Zhang, "Beyond a Gaussian Denoiser: Residual Learning of Deep CNN for Image Denoising," in IEEE Transactions on Image Processing, vol. 26, no. 7, pp. 3142-3155, July 2017, doi: 10.1109/TIP.2017.2662206.

U. S. Kamilov, C. A. Bouman, G. T. Buzzard and B. Wohlberg, "Plug-and-Play Methods for Integrating Physical and Learned Models in Computational Imaging: Theory, algorithms, and applications," in IEEE Signal Processing Magazine, vol. 40, no. 1, pp. 85-97, Jan. 2023, doi: 10.1109/MSP.2022.3199595.

Contour Detection and Hierarchical Image Segmentation P. Arbelaez, M. Maire, C. Fowlkes and J. Malik. IEEE TPAMI, Vol. 33, No. 5, pp. 898-916, May 2011.