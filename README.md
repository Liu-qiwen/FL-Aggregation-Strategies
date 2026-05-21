# 模型聚合权重对联邦学习的影响研究
联邦学习作为一种分布式机器学习范式，可以实现多个客户端在不共享本地数据的情况下，协作训练出高精度模型。在联邦学习的实际场景中，客户端之间的数据多为非独立同分布，此时全局模型在整体性能上面临着较大的挑战。作为影响模型性能的关键因素，模型聚合权重的设置直接影响了全局模型的性能。因此，本文针对数据异构场景下的联邦学习模型聚合权重设置展开了研究，对比了5种不同的模型聚合策略在数据高度异构场景下的表现。本实验利用狄利克雷分布对客户端数据进行划分，并基于卷积神经网络架构，在MNIST和CIFAR-10数据集上对5种聚合策略展开系统性地对比分析。实验结果表明，在处理MNIST基础任务时，上述5种聚合策略的收敛表现相近且精度较高，而在处理CIFAR-10复杂任务时，各聚合策略的表现具有显著的差异。样本量加权聚合和精度与样本量加权聚合策略在两种任务上表现均较好。本文的实验结果为联邦学习模型聚合优化方法的选择提供了一定的参考价值。

As a distributed machine learning paradigm, federated learning can enable multiple clients to collaborate to train high-precision models without sharing local data. In the actual scenario of federated learning, the data between clients is mostly non-independent and identically distributed, and the global model faces great challenges in overall performance. As a key factor affecting the performance of the model, the setting of model aggregation weight directly affects the performance of the global model. Therefore, this thesis focuses on the aggregation weight setting of federated learning model in the scenario of data heterogeneity, and compares the performance of five different model aggregation strategies in the scenario of highly heterogeneous data. In this experiment, the Dirichlet distribution is used to divide the client data, and the five aggregation strategies are systematically compared and analyzed on the MNIST and CIFAR-10 datasets based on the convolutional neural network architecture. Experimental results show that the above five aggregation strategies have similar convergence performance and high accuracy when dealing with the MNIST basic task, and there are significant differences in the performance of each aggregation strategy when dealing with the CIFAR-10 complex task. The sample size weighted aggregation and precision and sample size weighted aggregation strategies perform better on both tasks. The experimental results in this thesis provide some reference value for the selection of aggregation optimization methods for federated learning models.

## 实验一代码：MNIST数据集，随机选取40%客户端参与训练

https://www.kaggle.com/code/starwen/mnist-final?scriptVersionId=316249015

## 实验二代码：MNIST数据集，随机选取100%客户端参与训练

https://www.kaggle.com/code/starwen/mnist-final

## 实验三代码：CIFAR-10数据集，随机选取40%客户端参与训练

https://www.kaggle.com/code/huang2077/cifar-10-65-0-2

## 实验四代码：CIFAR-10数据集，随机选取100%客户端参与训练

### 等权重聚合策略：

https://www.kaggle.com/code/starwen/cifar-10-1-0-1-final?scriptVersionId=316410047

### 截断均值聚合策略：

https://www.kaggle.com/code/xxxxy3/cifar-10-1-0-1-final?scriptVersionId=316451790

### 样本量加权聚合策略：

https://www.kaggle.com/code/starwen/cifar-10-1-0-1-final?scriptVersionId=316373434

### 精度加权聚合策略：

https://www.kaggle.com/code/xxxxy3/cifar-10-1-0-1-final?scriptVersionId=316777795

### 精度与样本量加权聚合策略：

https://www.kaggle.com/code/xxxxy3/cifar-10-1-0-1-final?scriptVersionId=316719429

## 五种聚合策略在四组实验上的结果可视化代码：

https://www.kaggle.com/code/xxxxy3/cifar-1-0-mnist
