# Human Activity Recognition
This is a Human Activity Recognition repository intended for computer vision course at Cairo University

## Target 
- Literature Review on Past papers with Critcism of DataSets Types used
- Added on Contribution

## Papers Reviewed 
1. Cat et al 2015 with Doi : https://doi.org/10.1016/j.asoc.2015.01.025
2. Bevilacqua et al 2019 with Doi : https://arxiv.org/pdf/1906.01935.pdf
3. HaChoi Paper 2016 with Doi : https://doi.org/10.1109/IJCNN.2016.7727224
4. Parental 2017 with Doi : https://www.ncbi.nlm.nih.gov/pubmed/29060391
5. JanSun 2018 with Doi : https://www.hindawi.com/journals/js/2018/8580959/
6. David M. Burns et al 2020 with Doi: https://arxiv.org/pdf/2001.05517.pdf
7. Jianguang Huang et al 2020 with Doi : https://ieeexplore.ieee.org/abstract/document/9043535
8. Kasnesis et al 2018 with Doi : https://arxiv.org/abs/1811.00170
9. Lingjuan Lyu al 2017 with Doi : https://www.researchgate.net/publication/320883605_Privacy-Preserving_Collaborative_Deep_Learning_with_Application_to_Human_Activity_Recognition?enrichId=rgreq-11191b898a62b6b37d73081740a9304c-XXX&enrichSource=Y292ZXJQYWdlOzMyMDg4MzYwNTtBUzo1NTk0OTA0MDM5MTM3MjhAMTUxMDQwNDMxNTMxOQ%3D%3D&el=1_x_3&_esc=publicationCoverPdf
10. Panwar et al. 2015 with Doi : https://www.ncbi.nlm.nih.gov/pubmed/29060391
11. Our NN Contribution : NN_KFolds + NN_PCA

## Paper Findings
|      |               | Bevil | Catal  | David  | HaChoi | Jiang  | JianSun | JianSun(E) | Kas  | Ling | Pan  |NNKFolds|
|------| ------------- |:-----:|:------:|:-------|:-------|:------:|:-------:|:----------:|:----:|:----:|:----:|:------:|
| LOSO | MHealth       | 85.00%| 95.87% | 91.78% | 75.69% | 93.81% | 78.48%  |  81.57%    |93.81%|92.05%|09.01%| 96.60% |
| LOSO | USCHAD        | ------| 74.62% | ------ | ------ | ------ | 59.13%  |  ------    |------|------|14.72%| 71.55% |
| LOSO | UTDMHAD1_1s   | ------| 31.98% | 30.33% | 19.49% | 32.60% | 18.97%  |  19.37%    |32.60%|36.73%|05.23%| 46.07% |
| LOSO | UTDMHAD2_1s   | ------| 73.67% | 64.96% | 59.58% | 71.02% | 51.17%  |  50.90%    |71.02%|74.77%|40.63%| 77.70% |
| LOSO | WHARF         | ------| 49.69% | 49.87% | 59.13% | 65.13% | 49.39%  |  50.52%    |65.13%|70.95%|------| 55.13% |
| LOSO | WISDM         | ------| 73.86% | ------ | 59.28% | ------ | ------  |  ------    |------|------|------| 68.37% |
| SNOW | MHealth       | 93.11%| 99.84% | 95.54% | 84.77% | 99.96% | ------  |  83.34%    |99.96%|99.77%|09.00%| 99.88% |
| SNOW | USCHAD        | ------| 91.18% | ------ | ------ | ------ | ------  |  ------    |------|------|13.84%| 92.13% |
| SNOW | UTDMHAD1_1s   | ------| 49.06% | 33.39% | 22.67% | 56.41% | ------  |  23.63%    |56.41%|61.53%|05.22%| 71.03% |
| SNOW | UTDMHAD2_1s   | ------| 81.07% | 69.05% | 61.67% | 84.62% | ------  |  56.06%    |84.62%|86.13%|51.59%| 87.97% |
| SNOW | WHARF         | ------| 66.42% | 62.40% | 68.95% | 87.45% | ------  |  57.06%    |87.45%|88.99%|------| 74.47% |
| SNOW | WISDM         | ------| 90.60% | 98.82% | 81.81% | 99.65% | ------  |  ------    |99.65%|99.47%|------| 97.19% |
| LOTO | MHealth       | 89.62%| 91.76% | 89.77% | 76.66% | 87.89% | 77.69%  |  80.27%    |87.89%|89.17%|09.02%| 93.87% |
| LOTO | USCHAD        | ------| 87.36% | ------ | ------ | 90.94% | ------  |  ------    |90.94%|------|13.85%| 88.85% |
| LOTO | UTDMHAD1_1s   | ------| 47.96% | 33.64% | 21.46% | 53.97% | 24.30%  |  27.46%    |53.97%|57.10%|05.24%| 71.09% |
| LOTO | UTDMHAD2_1s   | ------| 80.35% | 69.02% | 63.87% | 82.44% | ------  |  48.44%    |82.44%|83.64%|50.00%| 87.87% |
| LOTO | WHARF         | ------| 63.87% | 61.59% | 64.68% | 83.47% | ------  |  61.92%    |83.47%|85.07%|------| 71.29% |
| LOTO | WISDM         | ------| 80.11% | ------ | 76.42% | 91.02% | ------  |  ------    |91.02%|89.19%|------| 77.54% |
| FNOW | MHealth       | 95.96%| 99.55% | 93.65% | 79.85% | 99.70% | 78.77%  |  62.20%    |99.70%|99.33%|08.99%| 99.55% |
| FNOW | USCHAD        | ------| 88.79% | ------ | ------ | 91.55% | ------  |  ------    |91.55%|89.92%|13.50%| 91.05% |
| FNOW | UTDMHAD1_1s   | ------| 47.01% | 26.46% | 18.92% | 45.99% | 22.70%  |  19.79%    |45.99%|52.27%|05.27%| 70.29% |
| FNOW | UTDMHAD2_1s   | ------| 80.32% | 65.55% | 57.94% | 79.76% | 39.87%  |  37.46%    |79.76%|80.21%|48.04%| 89.12% |
| FNOW | WHARF         | ------| 60.76% | 57.70% | 61.70% | 78.49% | 44.43%  |  49.18%    |78.49%|83.29%|------| 69.27% |
| FNOW | WISDM         | ------| 88.84% | 96.46% | 77.07% | 99.06% | ------  |  ------    |99.06%|98.46%|------| 95.80% |
| ---- | OPPORTUNITY   | 86.68%| 85.45% | ------ | ------ | ------ | 83.21%  |  83.48%    |------|------|84.22%| ------ |
| ---- | FUSMPA        | ------| 96.02% | ------ | ------ | ------ | ------  |  ------    |------|------|------| ------ |
| HHAR | Overlapping   | ------| 23.69% | ------ | ------ | ------ | ------  |  ------    |------|------|18.80%| ------ |
| HHAR | Non-Overlapp  | ------| 28.13% | ------ | ------ | ------ | ------  |  ------    |------|------|------| ------ |
