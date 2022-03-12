# Network
神经网络与深度学习 学习过程
====
武汉工程大学计算机学院 智能科学与技术
```python
import mnist_loader

training_data, validation_data, test_data = \
mnist_loader.load_data_wrapper()

import network
net = network.Network([784, 100, 10])
net.SGD(training_data, 30, 10, 1.0, test_data=test_data)
```
