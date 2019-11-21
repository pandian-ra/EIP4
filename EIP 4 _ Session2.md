# Session 2 Assignment

### 1.Logs for 20 epochs
Train on 60000 samples, validate on 10000 samples
Epoch 1/20

Epoch 00001: LearningRateScheduler setting learning rate to 0.003.
60000/60000 [==============================] - 47s 783us/step - loss: 0.3774 - acc: 0.9048 - val_loss: 0.0673 - val_acc: 0.9825
Epoch 2/20

Epoch 00002: LearningRateScheduler setting learning rate to 0.0022744503.
60000/60000 [==============================] - 44s 732us/step - loss: 0.1447 - acc: 0.9619 - val_loss: 0.0497 - val_acc: 0.9862
Epoch 3/20

Epoch 00003: LearningRateScheduler setting learning rate to 0.0018315018.
60000/60000 [==============================] - 45s 756us/step - loss: 0.1094 - acc: 0.9707 - val_loss: 0.0365 - val_acc: 0.9891
Epoch 4/20

Epoch 00004: LearningRateScheduler setting learning rate to 0.0015329586.
60000/60000 [==============================] - 45s 745us/step - loss: 0.0895 - acc: 0.9763 - val_loss: 0.0315 - val_acc: 0.9904
Epoch 5/20

Epoch 00005: LearningRateScheduler setting learning rate to 0.0013181019.
60000/60000 [==============================] - 45s 749us/step - loss: 0.0766 - acc: 0.9784 - val_loss: 0.0331 - val_acc: 0.9900
Epoch 6/20

Epoch 00006: LearningRateScheduler setting learning rate to 0.0011560694.
60000/60000 [==============================] - 44s 727us/step - loss: 0.0708 - acc: 0.9805 - val_loss: 0.0358 - val_acc: 0.9893
Epoch 7/20

Epoch 00007: LearningRateScheduler setting learning rate to 0.0010295127.
60000/60000 [==============================] - 44s 738us/step - loss: 0.0617 - acc: 0.9830 - val_loss: 0.0278 - val_acc: 0.9919
Epoch 8/20

Epoch 00008: LearningRateScheduler setting learning rate to 0.0009279307.
60000/60000 [==============================] - 44s 740us/step - loss: 0.0580 - acc: 0.9842 - val_loss: 0.0263 - val_acc: 0.9923
Epoch 9/20

Epoch 00009: LearningRateScheduler setting learning rate to 0.0008445946.
60000/60000 [==============================] - 45s 749us/step - loss: 0.0567 - acc: 0.9841 - val_loss: 0.0216 - val_acc: 0.9943
Epoch 10/20

Epoch 00010: LearningRateScheduler setting learning rate to 0.0007749935.
60000/60000 [==============================] - 45s 749us/step - loss: 0.0560 - acc: 0.9844 - val_loss: 0.0249 - val_acc: 0.9931
Epoch 11/20

Epoch 00011: LearningRateScheduler setting learning rate to 0.0007159905.
60000/60000 [==============================] - 44s 740us/step - loss: 0.0514 - acc: 0.9852 - val_loss: 0.0217 - val_acc: 0.9936
Epoch 12/20

Epoch 00012: LearningRateScheduler setting learning rate to 0.000665336.
60000/60000 [==============================] - 44s 727us/step - loss: 0.0508 - acc: 0.9856 - val_loss: 0.0207 - val_acc: 0.9943
Epoch 13/20

Epoch 00013: LearningRateScheduler setting learning rate to 0.0006213753.
60000/60000 [==============================] - 44s 731us/step - loss: 0.0470 - acc: 0.9866 - val_loss: 0.0220 - val_acc: 0.9939
Epoch 14/20

Epoch 00014: LearningRateScheduler setting learning rate to 0.0005828638.
60000/60000 [==============================] - 45s 755us/step - loss: 0.0477 - acc: 0.9864 - val_loss: 0.0206 - val_acc: 0.9940
Epoch 15/20

Epoch 00015: LearningRateScheduler setting learning rate to 0.0005488474.
60000/60000 [==============================] - 45s 754us/step - loss: 0.0462 - acc: 0.9867 - val_loss: 0.0209 - val_acc: 0.9939
Epoch 16/20

Epoch 00016: LearningRateScheduler setting learning rate to 0.0005185825.
60000/60000 [==============================] - 45s 746us/step - loss: 0.0436 - acc: 0.9876 - val_loss: 0.0204 - val_acc: 0.9940
Epoch 17/20

Epoch 00017: LearningRateScheduler setting learning rate to 0.000491481.
60000/60000 [==============================] - 43s 723us/step - loss: 0.0436 - acc: 0.9871 - val_loss: 0.0196 - val_acc: 0.9944
Epoch 18/20

Epoch 00018: LearningRateScheduler setting learning rate to 0.0004670715.
60000/60000 [==============================] - 44s 726us/step - loss: 0.0443 - acc: 0.9872 - val_loss: 0.0189 - val_acc: 0.9943
Epoch 19/20

Epoch 00019: LearningRateScheduler setting learning rate to 0.0004449718.
60000/60000 [==============================] - 45s 751us/step - loss: 0.0418 - acc: 0.9883 - val_loss: 0.0192 - val_acc: 0.9948
Epoch 20/20

Epoch 00020: LearningRateScheduler setting learning rate to 0.000424869.
60000/60000 [==============================] - 45s 752us/step - loss: 0.0407 - acc: 0.9881 - val_loss: 0.0182 - val_acc: 0.9947
<keras.callbacks.History at 0x7f497c52c780>

### 2. model.evaluate : [0.0181614178378135, 0.9947]
### 3. Stretegy:
1. I've used Dropout after every convolution except at the last layer. The accuracy has been increased when I don't use dropout at the last layer and i believe the reason is at the last layer, we need to preserve the weights at the last layer for better decisions.
2. I used a 3x3 convolution followed by 1x1 convolution as a batch inspired by ResNet Arch. Which decreased the parameters and also increased accuracy.
3. Usual thing. I used 2x2 Maxpooling to decrease the parameters and decrease the size of image.
4. I've increased the dropout rate to 0.2 to increase more accuracy.
### 4. Parameter: 
Total params: 14,352
Trainable params: 14,108
Non-trainable params: 244
__________________________