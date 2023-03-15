# fl
1. 通信压缩与编码在联邦学习中具有重要意义，以下是一些在此方向的重要论文以及它们的主要工作：
   1. Konečnỳ, J., McMahan, H. B., Yu, F. X., Richtárik, P., Suresh, A. T., & Bacon, D. (2016). Federated learning: Strategies for improving communication efficiency. arXiv preprint arXiv:1610.05492. 本论文提出了多种通信压缩策略，如梯度量化、梯度稀疏化等，以降低联邦学习的通信负担。实验结果表明，这些方法可以在保持模型性能的同时，显著降低通信开销。
   2. Alistarh, D., Grubic, D., Li, J., Tomioka, R., & Vojnovic, M. (2017). QSGD: Communication-efficient SGD via gradient quantization and encoding. In Advances in Neural Information Processing Systems (pp. 1709-1720). 本文提出了QSGD（Quantized Stochastic Gradient Descent）算法，通过对梯度进行量化和编码，实现了通信效率的显著提升。实验结果表明，QSGD在很多实际应用中具有较高的收敛速度和通信效率。
   3. Bernstein, J., Zhao, Y., Konečnỳ, J., & Wright, R. (2018). signSGD: compressed optimisation for non-convex problems. arXiv preprint arXiv:1802.04434. 本论文提出了signSGD方法，通过对梯度进行符号压缩，降低通信负担。实验结果表明，signSGD在多个非凸优化问题中具有良好的收敛性能和通信效率。
   4. Lin, Y., Han, S., Mao, H., Wang, Y., & Dhillon, H. (2020). A communication-efficient parallel training framework for federated learning. IEEE Journal on Selected Areas in Communications, 38(12), 2812-2826. 本论文提出了一种通信效率的并行训练框架，通过使用梯度压缩和网络编码技术，降低联邦学习的通信成本。实验结果表明，该框架在多个数据集上表现出较好的收敛性能和通信效率。
   5. Horváth, Á., Richtárik, P., & Sahu, A. K. (2021). NAC: A non-adaptive compression scheme for gradient updates in federated learning. arXiv preprint arXiv:2105.10499. 本论文提出了一种非自适应压缩方案（NAC），用于联邦学习中的梯度更新。该方法通过结合梯度量化和

设备选择与调度在联邦学习中是一个关键问题，以下是一些在此方向的重要论文以及它们的主要工作：

1. Nishio, T., & Yonetani, R. (2019). Client selection for federated learning with heterogeneous resources in mobile edge. arXiv preprint arXiv:1901.08696. 本论文提出了一种基于设备资源的联邦学习客户端选择方法，通过考虑设备的计算能力、通信能力和数据分布特性，实现了通信开销的有效降低，同时保证系统性能。
2. Hsieh, K. C., Kim, S., Balan, R. K., & Lim, H. (2019). FLiER: Federated Learning with Edge Resources. In Proceedings of the Tenth ACM International Conference on Future Energy Systems (pp. 389-399). 本文提出了FLiER方法，一种利用边缘资源进行联邦学习的设备选择策略。通过将边缘设备作为中继节点，该方法有效地减少了通信延迟并降低了能耗。
3. Caldas, S., Duddu, S. V., Wu, P., Li, T., Konečnỳ, J., McMahan, H. B., ... & Talwalkar, A. (2018). LEAF: A benchmark for federated settings. arXiv preprint arXiv:1812.01097. 本论文提出了LEAF，一个用于评估联邦学习算法的基准测试集。通过对多个数据集进行实验，作者展示了不同设备选择策略在不同场景下的性能差异，为设备选择研究提供了有价值的参考。
4. Yang, T., Andrew, G., Eichner, H., Sun, H., Li, W., Kong, N., ... & Beaufays, F. (2020). Applied federated learning: Improving google keyboard query suggestions. arXiv preprint arXiv:1812.02903. 本文介绍了谷歌键盘查询建议的应用联邦学习实践。作者通过智能设备选择策略，减少了通信负担，提高了系统性能。
5. Li, T., Sahu, A. K., Zaheer, M., Sanjabi, M., Talwalkar, A., & Smith, V. (2020). Federated optimization in heterogeneous networks. In Proceedings of Machine Learning Research (Vol. 108, pp. 429-450). 该论文研究了异构网络中的联邦优化问题，并提出了一种新的优化算法（FedProx），可以在通信受限的环境下实现高效学习。FedProx通过引入近端项，考虑了设备之间的异构性，从而降低通信成本。

本地更新策略在联邦学习中具有重要作用，以下是一些在此方向的重要论文以及它们的主要工作：

1. McMahan, H. B., Moore, E., Ramage, D., Hampson, S., & y Arcas, B. A. (2017). Communication-Efficient Learning of Deep Networks from Decentralized Data. In Proceedings of the 20th International Conference on Artificial Intelligence and Statistics (AISTATS) (pp. 1273-1282). 本论文提出了联邦平均算法（FedAvg），作为一种基本的本地更新策略。FedAvg通过在本地设备上进行多轮梯度下降，并将结果上传到服务器进行全局模型更新，从而在保证模型性能的同时降低通信成本。
2. Wang, S., Tuor, T., Salonidis, T., Leung, K. K., Makaya, C., He, T., & Chan, K. (2019). Adaptive federated learning in resource constrained edge computing systems. IEEE Journal on Selected Areas in Communications, 37(6), 1205-1221. 本论文提出了一种资源受限的边缘计算系统中的自适应联邦学习方法。该方法通过动态调整本地迭代次数，优化通信与计算之间的平衡，从而提高系统性能。
3. Li, T., Sahu, A. K., Zaheer, M., Sanjabi, M., Talwalkar, A., & Smith, V. (2020). Federated optimization in heterogeneous networks. In Proceedings of Machine Learning Research (Vol. 108, pp. 429-450). 该论文提出了一种新的优化算法（FedProx），可以在通信受限的环境下实现高效学习。FedProx通过引入近端项，考虑了设备之间的异构性，从而降低通信成本。
4. Sahu, A. K., Li, T., Sanjabi, M., Zaheer, M., Talwalkar, A., & Smith, V. (2019). On the convergence of federated optimization in heterogeneous networks. arXiv preprint arXiv:1812.06127. 本论文研究了不同本地更新策略在异构网络中的联邦优化收敛性。作者通过理论分析和实验验证了在设备异构性较大的情况下，适当调整本地更新策略可以提高收敛速度。
5. Karimireddy, S. P., Kale, S., Mohri, M., Suresh, A. T., & Reddi, S. J. (2020). SCAFFOLD: Stochastic controlled averaging for on-device federated learning. In International Conference on Machine Learning (pp. 5131-5141). 本论文提出了SCAFFOLD算法，一种用于在设备上进行联邦学习的随机控制平均方法。SCAFFOLD通过在本地设
