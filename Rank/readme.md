
**Table I. Rank-based comparison for the ablation study [1].** Two ranking protocols are considered: (1) *Avg Rank (4 datasets)* computes the average rank across Waterbirds, CelebA, Texture, and PACS, where PACS is treated as a single dataset by averaging performance over its four domains before ranking; (2) *Avg Rank (15 settings)* treats each PACS source→target pair (12 in total) as an individual setting, together with the other three datasets. **N=64 and Training Loss are set to match the corresponding settings of MetaWeightNet (MW-Net).**

| Method | Ablation Component | Avg Rank (4 datasets) ↓ | Avg Rank (15 settings) ↓ |
|:-:|:-:|:-:|:-:|
| Ours (N=1024, Full Feature) | - | **1.50** | **1.93** |
| N=256 | Batch Size | 3.00 | 2.47 |
| N=64 (**Same as MW-Net**) | Batch Size | 3.50 | 3.73 |
| Raw Image        | Input Feature | 5.75 | 5.07 |
| ResNet Features  | Input Feature | 3.00 | 3.80 |
| Training Loss (**Same as MW-Net**)   | Input Feature | 4.25 | 3.87 |


---

**Table II. Average-accuracy comparison for the ablation study. N=64 and Training Loss are set to match the corresponding settings of MetaWeightNet (MW-Net).**

| Method | Ablation Component | Waterbirds | CelebA | Texture | PACS-Art | PACS-Cartoon | PACS-Photo | PACS-Sketch | Avg |
|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
| Ours<br>(N=1024, Full Feature) | – | 81.81 | **85.01** | 29.38 | **83.07** | **86.79** | **71.16** | **79.06** | **73.75** |
| N=256 | Batch Size | 81.64 | 84.68 | 27.81 | 82.86 | **86.79** | 67.32 | 77.66 | 72.68 |
| N=64<br> (**Same as MW-Net**) | Batch Size | **81.82** | 80.27 | 28.33 | 82.27 | 86.02 | 64.40 | 73.62 | 70.96 |
| Raw Image        | Input Feature | 78.78 | 73.63 | 24.31 | 80.53 | 85.30 | 60.44 | 74.38 | 68.20 |
| ResNet Features  | Input Feature | 80.60 | 83.39 | **29.72** | 82.23 | 86.19 | 67.82 | 72.47 | 71.77 |
| Training Loss<br> (**Same as MW-Net**)   | Input Feature | 72.63 | 78.28 | 28.96 | 82.44 | 85.09 | 63.45 | 78.10 | 69.85 |



[1] Demšar J. Statistical comparisons of classifiers over multiple data sets[J]. Journal of Machine learning research, 2006, 7(Jan): 1-30.

