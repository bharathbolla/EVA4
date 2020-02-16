# EVA4
## Session_4 Assignment

### Acheived final accuracy of 99.42 (13th epoch). Used Batchnorm, maxpool and  dropout. Experimented with dropout. Dropout with 0.05 is better than dropout with 0.10.
### Total number of parameters 12,400
### Total 7 conv2d layers.

Model Architecture
----------------------------------------------------------------
        Layer (type)               Output Shape         Param #
================================================================
            Conv2d-1           [-1, 16, 26, 26]             144
              ReLU-2           [-1, 16, 26, 26]               0
       BatchNorm2d-3           [-1, 16, 26, 26]              32
         Dropout2d-4           [-1, 16, 26, 26]               0
            Conv2d-5           [-1, 32, 24, 24]           4,608
              ReLU-6           [-1, 32, 24, 24]               0
       BatchNorm2d-7           [-1, 32, 24, 24]              64
         Dropout2d-8           [-1, 32, 24, 24]               0
            Conv2d-9            [-1, 8, 24, 24]             256
        MaxPool2d-10            [-1, 8, 12, 12]               0
           Conv2d-11           [-1, 16, 10, 10]           1,152
             ReLU-12           [-1, 16, 10, 10]               0
      BatchNorm2d-13           [-1, 16, 10, 10]              32
        Dropout2d-14           [-1, 16, 10, 10]               0
           Conv2d-15             [-1, 16, 8, 8]           2,304
             ReLU-16             [-1, 16, 8, 8]               0
      BatchNorm2d-17             [-1, 16, 8, 8]              32
        Dropout2d-18             [-1, 16, 8, 8]               0
           Conv2d-19             [-1, 16, 8, 8]           2,304
             ReLU-20             [-1, 16, 8, 8]               0
      BatchNorm2d-21             [-1, 16, 8, 8]              32
        Dropout2d-22             [-1, 16, 8, 8]               0
           Conv2d-23             [-1, 10, 6, 6]           1,440
        AvgPool2d-24             [-1, 10, 1, 1]               0
================================================================
Total params: 12,400
Trainable params: 12,400
Non-trainable params: 0
----------------------------------------------------------------

### Logs

0%|          | 0/469 [00:00<?, ?it/s]/usr/local/lib/python3.6/dist-packages/ipykernel_launcher.py:61: UserWarning: Implicit dimension choice for log_softmax has been deprecated. Change the call to include dim=X as an argument.
loss=0.06598751991987228 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 36.56it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0726, Accuracy: 9793/10000 (97.93%)

loss=0.027347147464752197 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 36.62it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0463, Accuracy: 9864/10000 (98.64%)

loss=0.05034703388810158 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 35.48it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0355, Accuracy: 9885/10000 (98.85%)

loss=0.031144654378294945 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 37.17it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0323, Accuracy: 9893/10000 (98.93%)

loss=0.030386915430426598 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 37.90it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0295, Accuracy: 9903/10000 (99.03%)

loss=0.045595601201057434 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 37.80it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0266, Accuracy: 9914/10000 (99.14%)

loss=0.06021428480744362 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 38.60it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0239, Accuracy: 9930/10000 (99.30%)

loss=0.012945418246090412 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 37.76it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0261, Accuracy: 9914/10000 (99.14%)

loss=0.030130648985505104 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 37.99it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0221, Accuracy: 9937/10000 (99.37%)

loss=0.01618483103811741 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 38.76it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0219, Accuracy: 9939/10000 (99.39%)

loss=0.00646848464384675 batch_id=468: 100%|██████████| 469/469 [00:11<00:00, 40.98it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0220, Accuracy: 9935/10000 (99.35%)

loss=0.060666266828775406 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 38.10it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0209, Accuracy: 9942/10000 (99.42%)

loss=0.04660661146044731 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 38.57it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0209, Accuracy: 9936/10000 (99.36%)

loss=0.0055316537618637085 batch_id=468: 100%|██████████| 469/469 [00:11<00:00, 39.44it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0198, Accuracy: 9941/10000 (99.41%)

loss=0.05176045373082161 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 38.66it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0198, Accuracy: 9942/10000 (99.42%)

loss=0.012497514486312866 batch_id=468: 100%|██████████| 469/469 [00:11<00:00, 39.83it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0199, Accuracy: 9939/10000 (99.39%)

loss=0.08359097689390182 batch_id=468: 100%|██████████| 469/469 [00:12<00:00, 38.82it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0204, Accuracy: 9924/10000 (99.24%)

loss=0.0114469975233078 batch_id=468: 100%|██████████| 469/469 [00:11<00:00, 39.41it/s]
  0%|          | 0/469 [00:00<?, ?it/s]
Test set: Average loss: 0.0201, Accuracy: 9932/10000 (99.32%)

loss=0.015213902108371258 batch_id=468: 100%|██████████| 469/469 [00:11<00:00, 39.59it/s]

Test set: Average loss: 0.0190, Accuracy: 9940/10000 (99.40%)
