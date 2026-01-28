# Weld defects classifier

Weld Defects Classifier is a robust, easy-to-use solution for identifying weld defects in radiographic images. A model is created using ResNet50 using dataset from [RIAWELC](https://github.com/stefyste/RIAWELC) consisting of over 24,000 labeled radiographic images.

**Test radiographic weld images in your browser**  
you can use the images in the samples folder and visit the Streamlit [Weld Defect App](https://huggingface.co/spaces/zferd/welding-defect-app). Simply upload an X-ray image and receive instant predictions on these four defect classes:  

Lack of Penetration **(LP)**   
Porosity **(PO)**   
Cracks **(CR)**  
No Defect **(ND)**

You can also [download the model](https://huggingface.co/zferd/welding-defect/tree/main/model) deployed in huggingface.

### Test Classification report (RESNET50)
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

---

I also implemented a model using the state-of-the-art YOLOv11 architecture, achieving exceptional accuracy with real-time inference speeds.

### Test Classification report (YOLOv11)
```

              precision    recall  f1-score   support

          CR     0.9909    0.9798    0.9853       446
          LP     0.9922    0.9987    0.9954       765
          ND     1.0000    0.9817    0.9907       600
          PO     0.9798    0.9968    0.9882       632

    accuracy                         0.9906      2443
   macro avg     0.9907    0.9893    0.9899      2443
weighted avg     0.9907    0.9906    0.9906      2443
```

### Yolo test result

Under the video folder there is a video file that shows YOLO's crack defects results from test dataset of RIAWELC. 

### Credits

[1] Benito Totino, Fanny Spagnolo, Stefania Perri, "RIAWELC: A Novel Dataset of Radiographic Images for Automatic Weld Defects Classification", in the Proceedings of the Interdisciplinary Conference on Mechanics, Computers and Electrics (ICMECE 2022), 6-7 October 2022, Barcelona, Spain.

[2] Stefania Perri, Fanny Spagnolo, Fabio Frustaci, Pasquale Corsonello, "Welding Defects Classification Through a Convolutional Neural Network", in press in Manufacturing Letters, Elsevier.
