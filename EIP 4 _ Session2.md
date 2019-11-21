# Session 2 Assignment

### 1.Logs for 20 epochs
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 49s 813us/step - loss: 0.4526 - acc: 0.8807 - val_loss: 0.1137 - val_acc: 0.9705
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 43s 716us/step - loss: 0.1927 - acc: 0.9483 - val_loss: 0.0810 - val_acc: 0.9773
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 43s 721us/step - loss: 0.1468 - acc: 0.9598 - val_loss: 0.0695 - val_acc: 0.9777
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 44s 726us/step - loss: 0.1279 - acc: 0.9645 - val_loss: 0.0497 - val_acc: 0.9864
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 43s 723us/step - loss: 0.1100 - acc: 0.9691 - val_loss: 0.0461 - val_acc: 0.9864
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 43s 719us/step - loss: 0.1012 - acc: 0.9709 - val_loss: 0.0415 - val_acc: 0.9877
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 43s 722us/step - loss: 0.0977 - acc: 0.9718 - val_loss: 0.0364 - val_acc: 0.9891
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 43s 723us/step - loss: 0.0910 - acc: 0.9740 - val_loss: 0.0369 - val_acc: 0.9886
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 43s 722us/step - loss: 0.0851 - acc: 0.9758 - val_loss: 0.0328 - val_acc: 0.9904
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 43s 719us/step - loss: 0.0823 - acc: 0.9768 - val_loss: 0.0345 - val_acc: 0.9900
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 44s 725us/step - loss: 0.0790 - acc: 0.9776 - val_loss: 0.0321 - val_acc: 0.9892
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 44s 727us/step - loss: 0.0760 - acc: 0.9780 - val_loss: 0.0332 - val_acc: 0.9899
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 44s 728us/step - loss: 0.0744 - acc: 0.9784 - val_loss: 0.0315 - val_acc: 0.9896
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 44s 726us/step - loss: 0.0717 - acc: 0.9791 - val_loss: 0.0296 - val_acc: 0.9904
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 44s 728us/step - loss: 0.0701 - acc: 0.9795 - val_loss: 0.0311 - val_acc: 0.9899
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 43s 724us/step - loss: 0.0685 - acc: 0.9805 - val_loss: 0.0274 - val_acc: 0.9916
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 43s 721us/step - loss: 0.0651 - acc: 0.9810 - val_loss: 0.0285 - val_acc: 0.9904
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 44s 725us/step - loss: 0.0648 - acc: 0.9811 - val_loss: 0.0285 - val_acc: 0.9913
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 44s 729us/step - loss: 0.0665 - acc: 0.9806 - val_loss: 0.0273 - val_acc: 0.9912
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 43s 722us/step - loss: 0.0636 - acc: 0.9816 - val_loss: 0.0277 - val_acc: 0.9906
<keras.callbacks.History at 0x7f82eec1e9b0>

### 2. model.evaluate : [0.02115759316980839, 0.993]
### 3. Stretegy:
Maxpooling 
BatchNormalization()
1x1 convolution - 3 layers(reduce parameter)
Dropout(0.2)(increase accuracy)
LearningRateScheduler
### 4. Parameter: 
Total params: 14,352
Trainable params: 14,108
Non-trainable params: 244