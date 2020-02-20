# KNN(K-Nearest-Neighborhood)

> Supervised-learning, Classification

* Train_data를 별도로 학습하지 않고, 메모리에 들고다니면서 각각의 Test_data와의 L-Norm(일반적으로 L2 많이 사용)을 Loss로 측정하여 Loss가 가장 작은 class로 분류
* K의 숫자에 따라서 Test_data로부터 Loss가 작은 인근 K개를 비교하여 classification
* 별도의 학습이 일어나지 않기 때문에 Train시 소요시간은 적으나, Test시 시간이 많이 소요되어 실제 활용에는 부적합
* 변수간 단위가 다를 경우 반드시 Normalization 이후 알고리즘을 적용해야함

# Linear Classifier

> Supervised-learning, Classification

1. Score function
> s = f(x;W) = Wx

2. Loss function
> Softmax

> SVM(Support Vector Machine)

3. Regularization

4. Optimization  
  ~~Strategy #1 Random search~~  

    Strategy #2 Gradient Descent
      - Numerical gradient: approximate, slow, easy to write
        (실제로는 쓰이지 않으나, scale을 줄여서 디버깅할 때 유용)
      - Analytic gradient : exact, fast, error-prone
      
        Weights += -learning_rate * Gradients
  
      etc) Stochastic Gradient Descent(SGD)
      > 전체 Data를 다 학습하고 weight을 업데이트 하지 않고, minibatch만 학습하고 weight를 업데이트
      * exact한 gradient를 구하는 것이 아닌 noise가 들어간 추정 gradient를 구하는 것이기 때문에 학습 속도가 느려질 수 있음
      * Momentum을 추가하면 성능이 더 좋아짐

<!--stackedit_data:
eyJoaXN0b3J5IjpbNzU1ODc5ODAxXX0=
-->