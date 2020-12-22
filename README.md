## Overview
This github is an implementation for accepted manuscript titled `Human Activity Recognition using Wearable Sensors: Review, Challenges, Evaluation Benchmark`.

Recognizing human activity plays a significant role in the advancements of human-interaction applications in healthcare, personal fitness, and smart devices. Many papers presented various techniques for human activity representation that resulted in distinguishable progress.

In this study, we conduct an extensive literature review on recent, top performing techniques in human activity recognition based on wearable sensors. Due to the lack of standardized evaluation and to assess and ensure a fair comparison between the state-of-the-art techniques, we applied a standardized evaluation benchmark on the state-of-the-art techniques using six publicly available data-sets: MHealth, USCHAD, UTDMHAD, WISDM, WHARF, and OPPORTUNITY. Also, we propose an experimental, improved approach that is a hybrid of enhanced handcrafted features and a neural network architecture which outperformed top-performing techniques with the same standardized evaluation benchmark applied concerning MHealth, USCHAD, UTD-MHAD data-sets.

## Contribution
Our work is reflected in the following contributions:

1. Extensive Literature review for recent, top-performing techniques in human
activity based on sensor data

2. Due to different evaluation methodologies, it is hard to achieve a fair comparison between recent techniques. Therefore, we applied a `standardized evaluation` benchmark on the recent works using `six` publicly available datasets with 3 different temporal windows techniques: `Full-Non-Overlapping`, `SemiNon-Overlapping`, and `Leave-One-Trial-Out`.
3. Implementation, training, and re-evaluation of the recent literature work using the proposed standardized evaluation benchmark so all techniques follow
the same experimental setup to ensure a fair comparison.
4. Proposal of an experimental, hybrid approach that combines enhanced feature extraction with neural networks, and evaluation using the proposed
evaluation benchmark criteria, achieving a competitive accuracy.

## Standardized Evaluation Benchmark
Recent approaches implemented, trained and re-evaluated alongside our hybrid approach to follow the same experimental setupusing a standardized benchmark: 6 publicly available data-sets and 3 temporal window techniques.

### Open Source Datasets Used
1. MHealth
2. USC-HAD 
3. UTD-MHAD 
4. WISDM 
5. WHARF
6. OPPORTUNITY

### Supported Checklist Temporal Window Generation Technique for datasets

![Alt text](Images/Checklist_Supported_Temporal_Window_Generation_Technique_Datasets.PNG?raw=true "Title")

## Evaluation Metric
We conducted our experiments using Google colab with 1xTesla T4 GPU, 2496 CUDA cores, and 12GB GDDR5 VRAM. In
our study, mean accuracy is taken into account as an evaluation criterion for results.


## Paper Findings
|      |               | Bevil | Catal  | David  | HaChoi | Xia    | JianSun | JianSun(E) | Kas  | Ling | Pan  |Prop. NN|
|------| ------------- |:-----:|:------:|:-------|:-------|:------:|:-------:|:----------:|:----:|:----:|:----:|:------:|
| LOSO | MHealth       | 85.00%| 95.87% | 91.78% | 75.69% | 93.81% | 78.48%  |  81.57%    |13.23%|92.05%|09.01%| 96.35% |
| LOSO | USCHAD        | ------| 74.62% | ------ | ------ | 32.60% | 59.13%  |  ------    |44.45%|------|14.72%| 74.71% |
| LOSO | UTDMHAD1_1s   | ------| 31.98% | 30.33% | 19.49% | ------ | 18.97%  |  19.37%    |06.68%|36.73%|05.23%| 50.82% |
| LOSO | UTDMHAD2_1s   | ------| 73.67% | 64.96% | 59.58% | 71.02% | 51.17%  |  50.90%    |18.40%|74.77%|40.63%| 81.37% |
| LOSO | WHARF         | ------| 49.69% | 49.87% | 59.13% | 65.13% | 49.39%  |  50.52%    |------|70.95%|------| 59.29% |
| LOSO | WISDM         | ------| 73.86% | ------ | 59.28% | 99.70% | ------  |  ------    |------|------|------| 77.91% |
| SNOW | MHealth       | 93.11%| 99.84% | 95.54% | 84.77% | 99.96% | ------  |  83.34%    |12.45%|99.77%|09.00%| 100.0% |
| SNOW | USCHAD        | ------| 91.18% | ------ | ------ | 56.41% | ------  |  ------    |39.48%|------|13.84%| 93.48% |
| SNOW | UTDMHAD1_1s   | ------| 49.06% | 33.39% | 22.67% | ------ | ------  |  23.63%    |06.85%|61.53%|05.22%| 71.62% |
| SNOW | UTDMHAD2_1s   | ------| 81.07% | 69.05% | 61.67% | 84.62% | ------  |  56.06%    |15.82%|86.13%|51.59%| 87.98% |
| SNOW | WHARF         | ------| 66.42% | 62.40% | 68.95% | 87.45% | ------  |  57.06%    |------|88.99%|------| 80.39% |
| SNOW | WISDM         | ------| 90.60% | 98.82% | 81.81% | 99.65% | ------  |  ------    |------|99.47%|------| 98.35% |
| LOTO | MHealth       | 89.62%| 91.76% | 89.77% | 76.66% | 87.89% | 77.69%  |  80.27%    |14.33%|89.17%|09.02%| 94.76% |
| LOTO | USCHAD        | ------| 87.36% | ------ | ------ | 90.94% | ------  |  ------    |40.61%|------|13.85%| 88.85% |
| LOTO | UTDMHAD1_1s   | ------| 47.96% | 33.64% | 21.46% | 53.97% | 24.30%  |  27.46%    |06.39%|57.10%|05.24%| 71.00% |
| LOTO | UTDMHAD2_1s   | ------| 80.35% | 69.02% | 63.87% | 82.44% | ------  |  48.44%    |18.13%|83.64%|50.00%| 87.18% |
| LOTO | WHARF         | ------| 63.87% | 61.59% | 64.68% | 83.47% | ------  |  61.92%    |------|85.07%|------| 77.20% |
| LOTO | WISDM         | ------| 80.11% | ------ | 76.42% | 91.02% | ------  |  ------    |------|89.19%|------| 86.18% |
| FNOW | MHealth       | 95.96%| 99.55% | 93.65% | 79.85% | 99.70% | 78.77%  |  62.20%    |09.52%|99.33%|08.99%| 99.70% |
| FNOW | USCHAD        | ------| 88.79% | ------ | ------ | 91.55% | ------  |  ------    |31.74%|89.92%|13.50%| 91.68% |
| FNOW | UTDMHAD1_1s   | ------| 47.01% | 26.46% | 18.92% | 45.99% | 22.70%  |  19.79%    |06.46%|52.27%|05.27%| 70.48% |
| FNOW | UTDMHAD2_1s   | ------| 80.32% | 65.55% | 57.94% | 79.76% | 39.87%  |  37.46%    |16.70%|80.21%|48.04%| 87.84% |
| FNOW | WHARF         | ------| 60.76% | 57.70% | 61.70% | 78.49% | 44.43%  |  49.18%    |------|83.29%|------| 76.02% |
| FNOW | WISDM         | ------| 88.84% | 96.46% | 77.07% | 99.06% | ------  |  ------    |------|98.46%|------| 97.50% |
| ---- | OPPORTUNITY   | 86.68%| 85.45% | ------ | ------ | ------ | 83.21%  |  83.48%    |------|------|84.22%| 86.77% |
| ---- | FUSMPA        | ------| 96.02% | ------ | ------ | ------ | ------  |  ------    |------|------|------| ------ |
| HHAR | Overlapping   | ------| 23.69% | ------ | ------ | ------ | ------  |  ------    |------|------|18.80%| ------ |
| HHAR | Non-Overlapp  | ------| 28.13% | ------ | ------ | ------ | ------  |  ------    |------|------|------| ------ |
