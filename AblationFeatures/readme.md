

**Table 1. Ablation study on local and global features.** Removing either local or global features consistently degrades performance across datasets, leading to average drops of 1.16% and 1.05%, respectively.

|Method|Waterbirds|CelebA|Texture|Art|Cartoon|Photo|Sketch|Avg|Δ vs Full|
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
|Ours (Full Features)|**81.81**|85.01|**29.38**|**83.07**|**86.79**|**71.16**|**79.06**|**73.75**|0.00|
|Ours (w/o Local)|79.91|**85.15**|27.71|82.58|86.01|69.21|77.61|72.59|-1.16|
|Ours (w/o Global)|81.27|83.51|28.60|81.53|86.58|69.26|78.19|72.70|-1.05|
