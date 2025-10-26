# Weld defects classifier

Weld Defects Classifier is a robust, easy-to-use solution for identifying weld defects in radiographic images. This repository features a deep learning model based on ResNet50, trained exclusively on the acclaimed [RIAWELC](https://github.com/stefyste/RIAWELC) dataset consisting of over 24,000 expertly labeled X-ray images.

Test radiographic weld images in your browser, you can use the images in the samples folder.  
Streamlit Webapp: https://weld-defect-j688m.ondigitalocean.app/

Simply upload an X-ray image and receive instant predictions on these four defect classes:  
Lack of Penetration **(LP)**   
Porosity **(PO)**   
Cracks **(CR)**  
No Defect **(ND)**

### Test Classification report
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
