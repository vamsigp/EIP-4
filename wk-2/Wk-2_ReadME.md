<b>Strategy </b>

Steps done to achieve desired Accuracy -

    - Base architecture from Eight_DNN notebook
    - Modified last 3 num of filters of the convolution layers
    - Added one more convolution layer with lesser number of filters
    - Modified Learning rate(slightly decreased from [this value is denominator 0.319 to 0.32])
 

As GlobalAverage pooling introduced in the class, tried replacing the last Flatten layer with GAP layer and ran the simulation. Am not sure if thats the correct way or not.

2 models are present in the Jupyter notebook
1. <b>Model-A (model) </b>
regualar CNN followed by BatchNormalization, Dropout and Maxpooling

<b> Result </b>

  <b><i>[0.01946080807595281, 0.9942]</i></b>
  

2. <b>Model-B (model_ga)</b>
Same as model-A except for the Flatten layer, GlobalAveragepooling is used
For evaluation only "model" needs to be considered.

<b> Result </b>

  <b><i>[0.020457593263906892, 0.9939]</i></b>

For the model-B Accuracy hists 99.4% for the intermediate epoch.

We can consider intermediate epoch model by means of callback and earlystopping. As they were not yet taught i didnt used them.

-----------------------------------------------------

<b>Log from the Model Training Data - </b>

Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 10s 170us/step - loss: 0.5491 - acc: 0.8463 - val_loss: 0.1194 - val_acc: 0.9793
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022727273.
60000/60000 [==============================] - 7s 120us/step - loss: 0.2585 - acc: 0.9222 - val_loss: 0.0567 - val_acc: 0.9874
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018292683.
60000/60000 [==============================] - 7s 122us/step - loss: 0.2034 - acc: 0.9393 - val_loss: 0.0411 - val_acc: 0.9911
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015306122.
60000/60000 [==============================] - 7s 119us/step - loss: 0.1724 - acc: 0.9459 - val_loss: 0.0409 - val_acc: 0.9909
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013157895.
60000/60000 [==============================] - 7s 118us/step - loss: 0.1559 - acc: 0.9495 - val_loss: 0.0350 - val_acc: 0.9917
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011538462.
60000/60000 [==============================] - 7s 118us/step - loss: 0.1409 - acc: 0.9517 - val_loss: 0.0341 - val_acc: 0.9914
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010273973.
60000/60000 [==============================] - 7s 120us/step - loss: 0.1304 - acc: 0.9535 - val_loss: 0.0280 - val_acc: 0.9922
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009259259.
60000/60000 [==============================] - 7s 119us/step - loss: 0.1249 - acc: 0.9534 - val_loss: 0.0260 - val_acc: 0.9922
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008426966.
60000/60000 [==============================] - 7s 120us/step - loss: 0.1185 - acc: 0.9545 - val_loss: 0.0248 - val_acc: 0.9926
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007731959.
60000/60000 [==============================] - 7s 118us/step - loss: 0.1148 - acc: 0.9548 - val_loss: 0.0298 - val_acc: 0.9921
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007142857.
60000/60000 [==============================] - 7s 119us/step - loss: 0.1120 - acc: 0.9538 - val_loss: 0.0251 - val_acc: 0.9933
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.0006637168.
60000/60000 [==============================] - 7s 118us/step - loss: 0.1093 - acc: 0.9542 - val_loss: 0.0206 - val_acc: 0.9938
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006198347.
60000/60000 [==============================] - 7s 118us/step - loss: 0.1046 - acc: 0.9568 - val_loss: 0.0215 - val_acc: 0.9940
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005813953.
60000/60000 [==============================] - 7s 119us/step - loss: 0.1038 - acc: 0.9549 - val_loss: 0.0210 - val_acc: 0.9947
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005474453.
60000/60000 [==============================] - 7s 118us/step - loss: 0.1008 - acc: 0.9580 - val_loss: 0.0187 - val_acc: 0.9944
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005172414.
60000/60000 [==============================] - 7s 117us/step - loss: 0.0992 - acc: 0.9568 - val_loss: 0.0195 - val_acc: 0.9940
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.0004901961.
60000/60000 [==============================] - 7s 119us/step - loss: 0.0982 - acc: 0.9580 - val_loss: 0.0197 - val_acc: 0.9939
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004658385.
60000/60000 [==============================] - 7s 119us/step - loss: 0.0982 - acc: 0.9569 - val_loss: 0.0200 - val_acc: 0.9937
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.000443787.
60000/60000 [==============================] - 7s 119us/step - loss: 0.0936 - acc: 0.9586 - val_loss: 0.0182 - val_acc: 0.9945
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.0004237288.
60000/60000 [==============================] - 7s 118us/step - loss: 0.0961 - acc: 0.9565 - val_loss: 0.0195 - val_acc: 0.9942
