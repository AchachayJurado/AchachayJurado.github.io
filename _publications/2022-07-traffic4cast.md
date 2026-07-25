---
title: "Traffic4cast at NeurIPS 2021-Temporal and Spatial Few-Shot Transfer Learning in Gridded Geo-Spatial Processes"
collection: publications
permalink: /publication/2022-07-traffic4cast
excerpt: 'traffic prediction, GNN'
date: 2022-07-20
venue: 'NeurIPS 2021 Competitions and Demonstrations Track'
paperurl:
citation:
---

<b>Abstract---</b> The IARAI Traffic4cast competitions at NeurIPS 2019 and 2020 showed that neural networks can 
successfully predict future traffic conditions 1 hour into the future on simply aggregated GPS probe data in time and 
space bins. We thus reinterpreted the challenge of forecasting traffic conditions as a movie completion task. U-Nets 
proved to be the winning architecture, demonstrating an ability to extract relevant features in this complex real-world 
geo-spatial process. Building on the previous competitions, Traffic4cast 2021 now focuses on the question of model 
robustness and generalizability across time and space. Moving from one city to an entirely different city, or moving 
from pre-COVID times to times after COVID hit the world thus introduces a clear domain shift. We thus, for the first 
time, release data featuring such domain shifts. The competition now covers ten cities over 2 years, providing data 
compiled from over 1012 GPS probe data. Winning solutions captured traffic dynamics sufficiently well to even cope with 
these complex domain shifts. Surprisingly, this seemed to require only the previous 1h traffic dynamic history and 
static road graph as input.

[Download paper here](https://proceedings.mlr.press/v176/eichenberger22a/eichenberger22a.pdf)

Cited as:

```
@inproceedings{eichenberger2022traffic4cast,
  title={Traffic4cast at NeurIPS 2021-Temporal and Spatial Few-Shot Transfer Learning in Gridded Geo-Spatial Processes},
  author={Eichenberger, Christian and Neun, Moritz and Martin, Henry and Herruzo, Pedro and Spanring, Markus and Lu, Yichao and Choi, Sungbin and Konyakhin, Vsevolod and Lukashina, Nina and Shpilman, Aleksei and others},
  booktitle={NeurIPS 2021 Competitions and Demonstrations Track},
  pages={97--112},
  year={2022},
  organization={PMLR}
}
```
