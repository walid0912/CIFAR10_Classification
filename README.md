# CIFAR10 Classification
Image Classification on CIFAR10 Dataset using CNNs, Python and Tensorflow 

# CIFAR10 Dataset
Le jeu de données CIFAR-10 est composé de 60 000 images couleur 32x32 réparties en 10 classes, avec 6 000 images par classe. Il y a 50000 images d'entraînement et 10000 images de test.

# Data Augmentation


# Architecture CNN 

| Layer (type)   |        Output Shape     |        Param #|
| :---         |     :---:      |          ---: |
| conv2d (Conv2D)   |          (None, 32, 32, 32)   |     896  |                                                                     
| activation (Activation)  |   (None, 32, 32, 32)    |    0         |                                                                
| batch_normalization (BatchNormalization) |  (None, 32, 32, 32)       128   |                                                                                          |conv2d_1 (Conv2D)      |     (None, 32, 32, 32)     |   9248      |                                                                 
|activation_1 (Activation)  | (None, 32, 32, 32)    |    0       |                                                                 
|batch_normalization_1 (BatchNormalization) | (None, 32, 32, 32)  |     128   |                                                                    
|max_pooling2d (MaxPooling2D)   |  (None, 16, 16, 32)    |   0     |                                                                                                   |dropout (Dropout)     |      (None, 16, 16, 32)   |     0         |
|conv2d_2 (Conv2D)    |       (None, 16, 16, 64)   |     18496    | 
|activation_2 (Activation)  | (None, 16, 16, 64)   |     0       |  
|batch_normalization_2 (BatchNormalization) |  (None, 16, 16, 64)  |     256 |      
|conv2d_3 (Conv2D)    |       (None, 16, 16, 64)   |     36928     |
|activation_3 (Activation)  | (None, 16, 16, 64)  |      0      |   
|batch_normalization_3 (BatchNormalization) |  (None, 16, 16, 64)   |    256    |   
|max_pooling2d_1 (MaxPooling2D) |(None, 8, 8, 64)   |      0   |      
|dropout_1 (Dropout)      |   (None, 8, 8, 64)     |     0      |   
| conv2d_4 (Conv2D)    |       (None, 8, 8, 128)   |      73856    | 
|activation_4 (Activation)  | (None, 8, 8, 128)    |     0        | 
|batch_normalization_4 (BatchNormalization) |  (None, 8, 8, 128)   |     512       |
|conv2d_5 (Conv2D)      |     (None, 8, 8, 128)    |     147584    |
|activation_5 (Activation)   |(None, 8, 8, 128)   |      0      |   
|batch_normalization_5 (BatchNormalization) |  (None, 8, 8, 128)  |      512   |    
|max_pooling2d_2 (MaxPooling2D)| (None, 4, 4, 128) |       0   |      
|dropout_2 (Dropout)  |       (None, 4, 4, 128)  |       0     |    
|flatten (Flatten)| (None, 2048)    |          0         |
|dense (Dense)    |           (None, 10)     |           20490|

# Results

