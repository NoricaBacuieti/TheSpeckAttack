# TheSpeckAttack

Here you will find the jupyter-notebooks for conducting the experiments described in my thesis:   
Deep Neural Networks aiding Cryptanalysis: A Case Study of the Speck Distinguisher

## Content

1. TheSpeckAttack_OneShot_and_Iterative_Pruning.ipynb for creating Figures: 1, 2, 3, 4, 5, 6, 7, 8.
2. TheSpeckAttack_Depth_1_No_shortcut_distinguisher.ipynb for obtaining the results for Table 8.
3. TheSpeckAttack_Depth_1_No_shortcut_distinguisher.ipynb (adapting the number of filters/neurons as described in the thesis) for obtaining the results for Tables: 13, 14 
4. TheSpeckAttack_Prune_with_Surgeon_based_on_APoZ.ipynb for obtaining ther results for Tables: 9, 10, 11, 12.
5. TheSpeckAttack_Train_Autoencoders_and_Distinguishers_with_Preprocessing.ipynb for obtaining the results for Tables: 15, 16, 17.
6. DifferentArchitectures_Resnet50V1.ipynb for obtaining the results for Tables: 18, 19.
7. DifferentArchitectures_Resnet50V2.ipynb for obtaining the results for Tables: 20, 21.
8. DifferentArchitectures_Resnet101V1.ipynb for obtaining the results for Tables: 22, 23.
9. DifferentArchitectures_Resnet101V2.ipynb for obtaining the results for Tables: 24, 25.
10. DifferentArchitectures_Depth_50_101.ipynb for obtaining the results for Tables: 26, 27.
11. DifferentArchitectures_DenseNet121.ipynb for obtaining the results for Table 28.
12. DifferentArchitectures_DenseNet169.ipynb for obtaining the results for Table 29.
13. DifferentArchitectures_Xception.ipynb for obtaining the results for Table 30.
14. TheSpeckAttack_Activations.ipynb for creating Figures: 11, 12, 13, 14.
15. TheSpeckAttack_FeatureVisualization.ipynb for creating Figures: 15, 16, 17, 18.
16. For obtaining the results for Tables: 6, 7, you can directly refer to the code available here: https://github.com/agohr/deep_speck

The reduced network can be seen here: TheSpeckAttack_The_reduced_network.ipynb

There are also the demo's used for defending the thesis: 
1. Demo_TheSpeckAttack_OneShot_and_Iterative_Pruning.ipynb
2. Demo_TheSpeckAttack_The_reduced_network.ipynb
3. Demo_TheSpeckAttack_Train_Autoencoders_and_Distinguishers_with_Preprocessing.ipynb

## Setup

The experiments were run on an RTX 3090. 
Besides the experiments described in Section 4 regarding the evaluation of the Lottery Ticket Hypothesis that require around 24 hours (for the depth-10 network), and the experiments described in Section 6 that require around 48 hours per classification case to finish, all other experiments require from a few minutes to 2-3 hours.   

## Requirements

1. Tensorflow 2.4.0 (For TheSpeckAttack_Prune_with_Surgeon_based_on_APoZ.ipynb Tensorflow 2.2.0 is needed.)
2. Keras 2.4.0
3. Keract 4.4.0
4. LIME 0.2.0.1
5. Kerassurgeon 0.2.0
6. Lottery-ticket-pruner 0.8.1 

In addition, 24GB of RAM are needed to run the experiments described in Sections 5.2 and 6. 


## Acknowledgement

The above implementations make use of and adapt the code available at:

1. https://github.com/agohr/deep_speck
2. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/resnet.py#L439-L458
3. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/resnet_v2.py#L28-L56
4. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/resnet.py#L461-L479
5. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/resnet_v2.py#L59-L87
6. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/densenet.py#L323-L333
7. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/densenet.py#L336-L346 
8. https://github.com/tensorflow/tensorflow/blob/v2.5.0/tensorflow/python/keras/applications/xception.py#L46-L313

And use the following libraries:

1. https://pypi.org/project/keract/
2. https://pypi.org/project/lime/
3. https://pypi.org/project/kerassurgeon/
4. https://pypi.org/project/lottery-ticket-pruner/
