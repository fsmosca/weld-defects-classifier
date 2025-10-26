# Weld defects classifier

### Model Performance
The ResNet50-based classifier achieves high accuracy and balanced precision/recall on the [RIAWELC](https://github.com/stefyste/RIAWELC) test dataset. Below is the detailed classification report:

### Classification report
```

              precision    recall  f1-score   support

          CR     0.9071    0.9193    0.9131       446
          LP     0.9554    0.9242    0.9395       765
          ND     0.9433    0.9983    0.9700       600
          PO     0.9692    0.9446    0.9567       632

    accuracy                         0.9468      2443
   macro avg     0.9437    0.9466    0.9449      2443
weighted avg     0.9472    0.9468    0.9467      2443
```

### Credits

[1] Benito Totino, Fanny Spagnolo, Stefania Perri, "RIAWELC: A Novel Dataset of Radiographic Images for Automatic Weld Defects Classification", in the Proceedings of the Interdisciplinary Conference on Mechanics, Computers and Electrics (ICMECE 2022), 6-7 October 2022, Barcelona, Spain.

[2] Stefania Perri, Fanny Spagnolo, Fabio Frustaci, Pasquale Corsonello, "Welding Defects Classification Through a Convolutional Neural Network", in press in Manufacturing Letters, Elsevier.
