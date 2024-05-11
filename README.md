# Masters-Project
Analysis of stability and accuracy of permutation invariant embedding schemes for deep neural networks.


# About project
Permutation-invariant neural networks is a type of deep learning architecture that can recognize patterns in sets even if the inputs are in a different order. Many of these architectures have the separation property meaning that these architectures map distinct inputs to distinct outputs up to permutation. We call such networks separating permutation invariant neural networks (SPINNs).
To ensure the robustness (stability) of these neural architectures we want the neural network to be Bi-Lipschitz. For that, we analyzed the Bi-Lipschitz property of different types of permutation-invariant functions to see how well these functions can be used to create stable embeddings for SPINNs. We proved that the permutation-invariant embeddings obtained by the summation of smooth or piecewise smooth functions are not Bi-Lipschitz. Also, it is already known that embeddings that combine linear mappings and 1-dimensional sorting are injective and permutation invariant and that the Bi-Lipschitz constants can be characterized in terms of the singular values of the linear component of the embedding. We improved these results by proving injectivity with an embedding dimension lower by a factor of two than the previously known dimension and improved the estimates for the Bi-Lipschitz constants of these embedding schemes.
We performed some experiments to analyze the stability and accuracy of the sorting-based SPINNs. These experiments produced some interesting observations and new insights into the stability and accuracy of the model. On our synthetic dataset, the model achieved high stability and accuracy even when the embedding dimension was very low compared to the required embedding dimension proved in our theoretical results.


# Observations: 


![Image Alt Text]([Screenshot 2024-05-11 at 12.13.26.jpeg](https://github.com/ravina029/Masters-Project/blob/main/Screenshot%202024-05-11%20at%2012.13.26.jpeg))

1. On our synthetic dataset, the model achieved high stability and accuracy even when the embedding dimension was very low compared to our theoretical result for the general data manifold. From these empirical results of the experiment, we found that the stability and accuracy of the model increases with the increase in the embedding dimension D keeping other parameters fixed, e.g. n = 100 and d = 3.

2. Stability of these embeddings increases with the size of the input dataset (synthetic).
3. Surprisingly, we found that there is no clear relationship between the input size or dimension and the accuracy of the model. This suggests that the accuracy of the embeddings is not as dependent on the size or dimension of the input dataset as it is on the value of the embedding dimension.
   
