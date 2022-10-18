# MetaDrive Multi-agent Environment Benchmark Results



* MetaDrive version: [0.2.5](https://github.com/metadriverse/metadrive/tree/releases/0.2.5)
* Training code: [CoPO repo](https://github.com/decisionforce/CoPO)
* Related project: [CoPO webpage](https://decisionforce.github.io/CoPO/)

**To DO:**

- [ ] Update checkpoints
- [ ] Deliver this page to other researchers that are looking for this

## Training Results

Learning curve:

![](figs/learning_curve.png)
![](figs/cl_learning_curve.png)

Success rate table:

|                    | Bottleneck    | Tollgate      | Intersection   | Roundabout   | Parking Lot   | PG Map        |
|:-------------------|:--------------|:--------------|:---------------|:-------------|:--------------|:--------------|
| IPPO               | 24.04 (18.74) | 4.41 (2.56)   | 71.91 (5.27)   | 66.43 (4.99) | 16.98 (5.90)  | 81.81 (6.50)  |
| CCPPO (Mean Field) | 14.60 (11.24) | 14.86 (16.47) | 70.79 (6.29)   | 71.03 (5.45) | 20.66 (3.47)  | 79.56 (3.92)  |
| CCPPO (Concat)     | 19.55 (15.80) | 3.53 (1.92)   | 75.67 (3.18)   | 67.82 (4.09) | 12.01 (7.52)  | 80.21 (3.58)  |
| CL                 | 78.80 (3.79)  | 37.90 (29.93) | 81.57 (2.95)   | 82.34 (3.35) | 31.16 (14.36) | 77.82 (24.85) |
| CoPO               | 47.39 (19.49) | 27.19 (25.63) | 79.47 (4.97)   | 72.82 (6.73) | 19.51 (5.59)  | 83.40 (3.13)  |


## Radar Figure


Please refer to XXXX notebook for code on how to draw radar figure.

If we run IPPO, CCPPO and CoPO for 1M environment steps (2M for CL):

![](figs/xxx.png)

If we run IPPO, CCPPO and CoPO for 5M environment steps:

![](figs/xxx.png)


## Training and Evaluation Scripts


We run 5 algorithms in 6 multi-agent environments. Each experiment is repeated 8 times. The training scripts are provided in:  https://github.com/decisionforce/CoPO/tree/main/copo_code/copo

Evaluation script is provided in:  https://github.com/decisionforce/CoPO/blob/main/copo_code/copo/eval.py

Please refer to [CoPO repo](https://decisionforce.github.io/CoPO/) for more information.



## Data

The compressed evaluation results that you can use to draw figure are provided in: XXXX

You can download the raw evaluation results here:  https://github.com/metadriverse/metadrive-benchmark/releases/tag/asset-marl

The compressed training log that you can use to draw learning curves are provided here: 
https://github.com/metadriverse/metadrive-benchmark/releases/download/asset-marl/training_curves.zip


Due to the huge volumn of the training results, we can not provide the raw training results and intermediate checkpoints. We select the best checkpoints and upload them to:  XXXX  You can also find them in the CoPO repo where you can XXXX them with XXXX.



## Reference

Please cite MetaDrive paper via: https://github.com/metadriverse/metadrive#-references

Please cite CoPO paper via: https://github.com/decisionforce/CoPO#citation
