<h3>Studying the effects of different initializers on Ensembling</h3>

<quote>The hypothesis proposed that since the initialization method decides how the model steps down the loss landscape, an ensemble of different types of initialization methods will lead to better overall scores.</quote>

The study was carried out on the CIFAR-10 dataset because of it's medium complexity and assured replicability

The initialization techniques involved:
1. Glorot Initializer (Default keras initializer)
2. He Initializer (<a href="https://arxiv.org/pdf/1502.01852.pdf">Here</a>)
3. Lecun Intializer (<a href="http://yann.lecun.com/exdb/publis/pdf/lecun-98b.pdf">Here</a>)

<h3>Training Graphs</h3>

![](https://github.com/DarshanDeshpande/Research-With-TF/Ensembling-of-different-initializers/blob/master/Graphs/Graph2.png)

![](https://github.com/DarshanDeshpande/Research-With-TF/Ensembling-of-different-initializers/blob/master/Graphs/Graph1.png)


<h3>Final Results</h3>
-------------------------------------------------------------------------------
Accuracy for mixed ensemble: 0.8351, Accuracies for individual models: [0.7672, 0.7502, 0.8057, 0.8044, 0.8082, 0.8092]
Accuracy for mixed ensemble: 0.8357, Accuracies for individual models: [0.7671, 0.7576, 0.8021, 0.8004, 0.803, 0.8151]
Accuracy for mixed ensemble: 0.834, Accuracies for individual models: [0.7656, 0.7637, 0.8044, 0.8045, 0.8153, 0.8118]
Accuracy for mixed ensemble: 0.8332, Accuracies for individual models: [0.77, 0.7647, 0.8053, 0.8075, 0.8139, 0.8042]
Accuracy for mixed ensemble: 0.8334, Accuracies for individual models: [0.7679, 0.7623, 0.7941, 0.8133, 0.8151, 0.8083]

Accuracy for Glorot Uniform Ensemble: 0.7895
Accuracy for He Uniform Ensemble: 0.8345
Accuracy for Lecun Uniform Ensemble: 0.842
Accuracy for Glorot Normal Ensemble: 0.7878
Accuracy for He Normal Ensemble: 0.8373
Accuracy for Lecun Normal Ensemble: 0.8394

<h3>Conclusions</h3>
From the training results above, it is safe to conclude that we can reject the proposed hypothesis for this specific dataset.
The possible reasons for such results could be that the current model is under-parameterized to achieve a better score.
The hypothesis is still to be tested on a different datasets to check for specific use cases(if any). Any contribution to this will be welcomed
