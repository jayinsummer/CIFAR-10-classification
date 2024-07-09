# 📖 내용
Image Classificatoin을 위한 CNN을 디벨롭시키는 교과목 내 프로젝트입니다.

<img width="398" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/cb768497-5476-42cc-8b9e-99876ec758aa">
<hr/>

# 🙋🏻‍♀️ 디벨롭하기 위해 변경한 사항들
최종 결론을 짓기 전에 epoch을 30, 40, 50으로 늘려 각각 테스트해보았고, epoch 40과 50에서는 유의미한 결과를 얻지 못하였습니다. Loss값이 일정 지점에서부터 다시 증가하는 양상을 지녔던 것으로 보아, overfitting이 발생했다고 판단하였습니다. 따라서 다음과 같은 결론을 내렸습니다.
### 1. Data Augmentation
<img width="383" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/b4d2ca20-e9bb-42cc-9b3a-6fed472333b1">

### 2. Batch Size = 16
<img width="382" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/a0f16ffe-bf54-42de-b5ee-605cbca9ec69">

### 3. Network Architecture: VGG11
<img width="253" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/771a5bfb-76b2-42fa-b8e3-b2f651927c3c">

### 4. Optimizer: Adam, Learning Rate = 0.001
<img width="400" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/b1291b51-33c5-4377-a7ca-94c031dba886">

### 5. Scheduler: CosineAnnealingLR
<img width="397" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/b95c590b-86a9-4b12-a7fb-0e1d98a7579d">

### 6. Epoch = 30
<img width="383" alt="Untitled" src = "https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/e29d0b60-b1d5-4da9-b3c9-4f90c01af9a4">
<hr/>

# ✅ 최종 Accuracy 및 Loss
Accuracy: 87%, Loss: 0.011
<img width="305" alt="Untitled" src="https://github.com/jayinsummer/CIFAR-10-classification/assets/112365313/8532f25f-9742-41d0-9661-eb8ed30ccbc0">
