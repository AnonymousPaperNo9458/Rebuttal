

**Table 1. Rank-based comparison for the ablation study.** Following prior recommendations (Demsar, JMLR 2006), we report average ranks instead of mean performance to compare our method with its ablated variants. We consider two ranking protocols: (1) *Avg Rank (4 datasets)* computes the average rank across Waterbirds, CelebA, Texture, and PACS, where PACS is treated as a single dataset by averaging performance over its four domains before ranking; (2) *Avg Rank (15 settings)* treats each PACS source→target pair (12 in total) as an individual setting, together with the other three datasets.

| Method | Ablation Component | Avg Rank (4 datasets) ↓ | Avg Rank (15 settings) ↓ |
|:-:|:-:|:-:|:-:|
| Ours (N=1024, Full Feature) | - | **1.50** | **1.93** |
| N=256 | Batch Size | 3.00 | 2.47 |
| N=64  | Batch Size | 3.50 | 3.73 |
| Raw Image        | Input Feature | 5.75 | 5.07 |
| ResNet Features  | Input Feature | 3.00 | 3.80 |
| Training Loss    | Input Feature | 4.25 | 3.87 |
