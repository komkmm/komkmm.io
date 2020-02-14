# KNN(K-Nearest-Neighborhood)

> Supervised-learning, Classification

* Train_data를 별도로 학습하지 않고, 메모리에 들고다니면서 각각의 Test_data와의 L-Norm(일반적으로 L2 많이 사용)을 Loss로 측정하여 Loss가 가장 작은 class로 분류
* K의 숫자에 따라서 Test_data로부터 Loss가 작은 인근 K개를 비교하여 classification
* 별도의 학습이 일어나지 않기 때문에 Train시 소요시간은 적으나, Test시 시간이 많이 소요되어 실제 활용에는 부적합
* 변수간 단위가 다를 경우 반드시 Normalization 이후 알고리즘을 적용해야함


