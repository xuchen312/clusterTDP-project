# True Discovery Proportion Estimation for Cluster Extent Inference

Random field theory (RFT)-based cluster extent thresholding is one of the most widely used approaches for activation detection in neuroimaging. While powerful for finding regions with some activation, this approach does not allow any further quantification or localisation of signal. This page aims to introduce a new method **clusterTDP** that presents an improvement of the current RFT-based cluster extent inference by returning a lower bound for true discovery proportion (TDP) for every region, i.e. the proportion of truly active voxels in the region. The TDP-based inference can be used to quantify how widely spread the signal is within a brain region and avoid the spatial specificity paradox associated with the cluster inference approaches. 

## clusterTDP

The [paper]([https://doi.org/10.1016/j.neuroimage.2018.07.060](https://doi.org/10.1093/jrsssb/qkad067)) proposes a new method **clusterTDP** that calculates lower and upper bounds for TDP to improve upon the classic cluster inference, where the lower bound retains the error control guarantee but is conservative; the upper bound is more accurate, but at the cost of losing error control if the method does not fully converge.

* SPM extension  [[clusterTDP-SPM](https://github.com/xuchen312/clusterTDP-SPM)]
* FSL other toolbox [[clusterTDP-FSL](https://github.com/rmonajemi/fMRI)]
* Python library

## References

Goeman, J.J., Górecki, P., Monajemi, R., Chen, X., Nichols, T.E. and Weeda, W. (2023). Cluster extent inference revisited: quantification and localisation of brain activity. *Journal of the Royal Statistical Society Series B: Statistical Methodology*, 85(4):1128–1153. [[Paper](https://doi.org/10.1093/jrsssb/qkad067)]

## Any questions?

Please email xuchen312@gmail.com.
