[!TOC]

### Base Resnet Accuracy

File - "Cifar10_resnet.ipynb"

Dervied from https://keras.io/examples/cifar10_resnet/

84.93% at Epoch 48
 
85.20% at Epoch 50

- Total params: 274,442
- Trainable params: 273,066
- Non-trainable params: 1,376

### Modified Resnet Accuracy

File - "Cifar10_resnet_Trails.ipynb"

90.34% at Epoch 47

90.28% at Epoch 50

- Total params: 792,330
- Trainable params: 790,090
- Non-trainable params: 2,240

 - Model file = cifar10_ResNet20v1_model.039.0.9033.h5

#### Strategy
1. Modified Number of kernels
2. Modified Learning rate
3. Added Regularization by cutout
4. Modified Batch size to 64

#### Log

>
	Epoch 1/50
	Learning rate:  0.001
	782/782 [==============================] - 91s 116ms/step - loss: 1.7690 - acc: 0.4491 - val_loss: 1.8735 - val_acc: 0.4755

	Epoch 00001: val_acc improved from -inf to 0.47550, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.001.0.4755.h5
	Epoch 2/50
	Learning rate:  0.001
	782/782 [==============================] - 82s 105ms/step - loss: 1.3645 - acc: 0.5981 - val_loss: 1.5039 - val_acc: 0.5844

	Epoch 00002: val_acc improved from 0.47550 to 0.58440, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.002.0.5844.h5
	Epoch 3/50
	Learning rate:  0.001
	782/782 [==============================] - 82s 104ms/step - loss: 1.1848 - acc: 0.6603 - val_loss: 1.6669 - val_acc: 0.5889

	Epoch 00003: val_acc improved from 0.58440 to 0.58890, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.003.0.5889.h5
	Epoch 4/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 1.0788 - acc: 0.6996 - val_loss: 1.0892 - val_acc: 0.7071

	Epoch 00004: val_acc improved from 0.58890 to 0.70710, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.004.0.7071.h5
	Epoch 5/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 1.0151 - acc: 0.7255 - val_loss: 1.8921 - val_acc: 0.5497

	Epoch 00005: val_acc did not improve from 0.70710
	Epoch 6/50
	Learning rate:  0.001
	782/782 [==============================] - 82s 105ms/step - loss: 0.9618 - acc: 0.7439 - val_loss: 1.2266 - val_acc: 0.6801

	Epoch 00006: val_acc did not improve from 0.70710
	Epoch 7/50
	Learning rate:  0.001
	782/782 [==============================] - 82s 104ms/step - loss: 0.9191 - acc: 0.7577 - val_loss: 0.9644 - val_acc: 0.7487

	Epoch 00007: val_acc improved from 0.70710 to 0.74870, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.007.0.7487.h5
	Epoch 8/50
	Learning rate:  0.001
	782/782 [==============================] - 82s 104ms/step - loss: 0.8966 - acc: 0.7665 - val_loss: 0.8513 - val_acc: 0.7891

	Epoch 00008: val_acc improved from 0.74870 to 0.78910, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.008.0.7891.h5
	Epoch 9/50
	Learning rate:  0.001
	782/782 [==============================] - 82s 104ms/step - loss: 0.8668 - acc: 0.7782 - val_loss: 0.9950 - val_acc: 0.7461

	Epoch 00009: val_acc did not improve from 0.78910
	Epoch 10/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 0.8500 - acc: 0.7843 - val_loss: 0.8461 - val_acc: 0.7932

	Epoch 00010: val_acc improved from 0.78910 to 0.79320, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.010.0.7932.h5
	Epoch 11/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 0.8333 - acc: 0.7907 - val_loss: 0.9343 - val_acc: 0.7737

	Epoch 00011: val_acc did not improve from 0.79320
	Epoch 12/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 0.8098 - acc: 0.7990 - val_loss: 1.0454 - val_acc: 0.7368

	Epoch 00012: val_acc did not improve from 0.79320
	Epoch 13/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 103ms/step - loss: 0.7948 - acc: 0.8028 - val_loss: 0.8592 - val_acc: 0.7884

	Epoch 00013: val_acc did not improve from 0.79320
	Epoch 14/50
	Learning rate:  0.001
	782/782 [==============================] - 80s 103ms/step - loss: 0.7821 - acc: 0.8107 - val_loss: 0.8839 - val_acc: 0.7848

	Epoch 00014: val_acc did not improve from 0.79320
	Epoch 15/50
	Learning rate:  0.001
	782/782 [==============================] - 80s 103ms/step - loss: 0.7715 - acc: 0.8130 - val_loss: 0.7902 - val_acc: 0.8167

	Epoch 00015: val_acc improved from 0.79320 to 0.81670, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.015.0.8167.h5
	Epoch 16/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 103ms/step - loss: 0.7642 - acc: 0.8167 - val_loss: 1.2291 - val_acc: 0.7267

	Epoch 00016: val_acc did not improve from 0.81670
	Epoch 17/50
	Learning rate:  0.001
	782/782 [==============================] - 80s 103ms/step - loss: 0.7518 - acc: 0.8209 - val_loss: 0.9818 - val_acc: 0.7783

	Epoch 00017: val_acc did not improve from 0.81670
	Epoch 18/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 0.7428 - acc: 0.8244 - val_loss: 0.9869 - val_acc: 0.7674

	Epoch 00018: val_acc did not improve from 0.81670
	Epoch 19/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 103ms/step - loss: 0.7319 - acc: 0.8270 - val_loss: 0.8466 - val_acc: 0.8074

	Epoch 00019: val_acc did not improve from 0.81670
	Epoch 20/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 103ms/step - loss: 0.7248 - acc: 0.8316 - val_loss: 0.8770 - val_acc: 0.8009

	Epoch 00020: val_acc did not improve from 0.81670
	Epoch 21/50
	Learning rate:  0.001
	782/782 [==============================] - 81s 104ms/step - loss: 0.7168 - acc: 0.8342 - val_loss: 1.0310 - val_acc: 0.7704

	Epoch 00021: val_acc did not improve from 0.81670
	Epoch 22/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 103ms/step - loss: 0.6174 - acc: 0.8685 - val_loss: 0.6089 - val_acc: 0.8749

	Epoch 00022: val_acc improved from 0.81670 to 0.87490, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.022.0.8749.h5
	Epoch 23/50
	Learning rate:  0.0001
	782/782 [==============================] - 80s 103ms/step - loss: 0.5759 - acc: 0.8813 - val_loss: 0.5725 - val_acc: 0.8817

	Epoch 00023: val_acc improved from 0.87490 to 0.88170, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.023.0.8817.h5
	Epoch 24/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 103ms/step - loss: 0.5542 - acc: 0.8861 - val_loss: 0.5642 - val_acc: 0.8850

	Epoch 00024: val_acc improved from 0.88170 to 0.88500, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.024.0.8850.h5
	Epoch 25/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.5379 - acc: 0.8890 - val_loss: 0.5658 - val_acc: 0.8819

	Epoch 00025: val_acc did not improve from 0.88500
	Epoch 26/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.5227 - acc: 0.8940 - val_loss: 0.5731 - val_acc: 0.8830

	Epoch 00026: val_acc did not improve from 0.88500
	Epoch 27/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.5154 - acc: 0.8951 - val_loss: 0.5292 - val_acc: 0.8954

	Epoch 00027: val_acc improved from 0.88500 to 0.89540, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.027.0.8954.h5
	Epoch 28/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.5088 - acc: 0.8942 - val_loss: 0.5243 - val_acc: 0.8949

	Epoch 00028: val_acc did not improve from 0.89540
	Epoch 29/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.4935 - acc: 0.9001 - val_loss: 0.5192 - val_acc: 0.8959

	Epoch 00029: val_acc improved from 0.89540 to 0.89590, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.029.0.8959.h5
	Epoch 30/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.4890 - acc: 0.9007 - val_loss: 0.5037 - val_acc: 0.9000

	Epoch 00030: val_acc improved from 0.89590 to 0.90000, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.030.0.9000.h5
	Epoch 31/50
	Learning rate:  0.0001
	782/782 [==============================] - 81s 104ms/step - loss: 0.4815 - acc: 0.9014 - val_loss: 0.4968 - val_acc: 0.8976

	Epoch 00031: val_acc did not improve from 0.90000
	Epoch 32/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 104ms/step - loss: 0.4678 - acc: 0.9068 - val_loss: 0.4947 - val_acc: 0.9002

	Epoch 00032: val_acc improved from 0.90000 to 0.90020, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.032.0.9002.h5
	Epoch 33/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4634 - acc: 0.9081 - val_loss: 0.4949 - val_acc: 0.9012

	Epoch 00033: val_acc improved from 0.90020 to 0.90120, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.033.0.9012.h5
	Epoch 34/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4589 - acc: 0.9076 - val_loss: 0.4997 - val_acc: 0.9001

	Epoch 00034: val_acc did not improve from 0.90120
	Epoch 35/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 104ms/step - loss: 0.4537 - acc: 0.9115 - val_loss: 0.4920 - val_acc: 0.9018

	Epoch 00035: val_acc improved from 0.90120 to 0.90180, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.035.0.9018.h5
	Epoch 36/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 104ms/step - loss: 0.4588 - acc: 0.9088 - val_loss: 0.4938 - val_acc: 0.9022

	Epoch 00036: val_acc improved from 0.90180 to 0.90220, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.036.0.9022.h5
	Epoch 37/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4517 - acc: 0.9113 - val_loss: 0.4948 - val_acc: 0.9015

	Epoch 00037: val_acc did not improve from 0.90220
	Epoch 38/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4548 - acc: 0.9106 - val_loss: 0.4925 - val_acc: 0.9029

	Epoch 00038: val_acc improved from 0.90220 to 0.90290, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.038.0.9029.h5
	Epoch 39/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4502 - acc: 0.9123 - val_loss: 0.4927 - val_acc: 0.9033

	Epoch 00039: val_acc improved from 0.90290 to 0.90330, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.039.0.9033.h5
	Epoch 40/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4527 - acc: 0.9116 - val_loss: 0.4949 - val_acc: 0.9024

	Epoch 00040: val_acc did not improve from 0.90330
	Epoch 41/50
	Learning rate:  1e-05
	782/782 [==============================] - 81s 103ms/step - loss: 0.4519 - acc: 0.9098 - val_loss: 0.4921 - val_acc: 0.9017

	Epoch 00041: val_acc did not improve from 0.90330
	Epoch 42/50
	Learning rate:  1e-06
	782/782 [==============================] - 81s 103ms/step - loss: 0.4489 - acc: 0.9134 - val_loss: 0.4903 - val_acc: 0.9028

	Epoch 00042: val_acc did not improve from 0.90330
	Epoch 43/50
	Learning rate:  1e-06
	782/782 [==============================] - 81s 103ms/step - loss: 0.4488 - acc: 0.9127 - val_loss: 0.4917 - val_acc: 0.9025

	Epoch 00043: val_acc did not improve from 0.90330
	Epoch 44/50
	Learning rate:  1e-06
	782/782 [==============================] - 81s 104ms/step - loss: 0.4525 - acc: 0.9104 - val_loss: 0.4919 - val_acc: 0.9029

	Epoch 00044: val_acc did not improve from 0.90330
	Epoch 45/50
	Learning rate:  1e-06
	782/782 [==============================] - 81s 104ms/step - loss: 0.4514 - acc: 0.9121 - val_loss: 0.4918 - val_acc: 0.9021

	Epoch 00045: val_acc did not improve from 0.90330
	Epoch 46/50
	Learning rate:  1e-06
	782/782 [==============================] - 81s 103ms/step - loss: 0.4498 - acc: 0.9119 - val_loss: 0.4915 - val_acc: 0.9028

	Epoch 00046: val_acc did not improve from 0.90330
	Epoch 47/50
	Learning rate:  5e-07
	782/782 [==============================] - 81s 103ms/step - loss: 0.4473 - acc: 0.9132 - val_loss: 0.4906 - val_acc: 0.9034

	Epoch 00047: val_acc improved from 0.90330 to 0.90340, saving model to /content/gdrive/My Drive/saved_models/cifar10_ResNet20v1_model.047.0.9034.h5
	Epoch 48/50
	Learning rate:  5e-07
	782/782 [==============================] - 81s 104ms/step - loss: 0.4504 - acc: 0.9109 - val_loss: 0.4920 - val_acc: 0.9026

	Epoch 00048: val_acc did not improve from 0.90340
	Epoch 49/50
	Learning rate:  5e-07
	782/782 [==============================] - 81s 103ms/step - loss: 0.4456 - acc: 0.9124 - val_loss: 0.4921 - val_acc: 0.9031

	Epoch 00049: val_acc did not improve from 0.90340
	Epoch 50/50
	Learning rate:  5e-07
	782/782 [==============================] - 81s 103ms/step - loss: 0.4464 - acc: 0.9125 - val_loss: 0.4929 - val_acc: 0.9028

	Epoch 00050: val_acc did not improve from 0.90340
