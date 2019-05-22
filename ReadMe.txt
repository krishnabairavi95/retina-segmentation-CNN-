Hello, 

I have prepared a report for the project. (Document Name: 16725_report.pdf). It is in the ‘proj’ of my folder. Please take a look at it. I have explained the methodology with references and results (including Images and the final ROC curve).  

Please  follow the following steps while running my code, I will walk you through. 


1. As first step, please open preprocess.py present in the Code section of Proj folder. Please download the DRIVE dataset images that I have given in the first reference of the code or I have included sample train and test images in train_data and test_data folders to use it for quick test run. Please give in your file destinations accordingly. I have tried different preprocessing techniques using ITK and I have saved the preprocessed images in a .npz file which I will be using while training and testing. If you run the code, you should be able to see the images getting saved into a .npz file. However, I have included the preprocessed  train and test datasets namely data_train_final.npz and  data_test_final.npz in the folder proj. Please feel free to use them while running the training and testing python codes.


2. As a next step- training- please open the file retiseg_train.py from “ ksoundar/Proj/Code” pathway and run it. While training the model, please change the respective architectures to U-Net and Seg-net. I have put comments on the code in the start and in the corresponding places for understanding. I have included my references in comments in the code. I trained the model for 10 epochs in a GPU and I have included the trained models to the trained_model folder. You can access it by following the pathway : “ ksoundar/Proj/trained_model. The trained_model folder contains both U-Net and Seg-net trained models files ( namely unet_epoch10.h5, and seg_epoch10.h5)  which can be used for predictions 

3. For Testing the model and for predictions, please open the file retiseg_test.py from “ ksoundar/Proj/Code” pathway to run it. While testing the model, please do the corresponding changes mentioned in the initial comments of the code. The trained model unet_epoch10.h5, and seg_epoch10.h5 mentioned in the above step can be used for predictions. The code will plot a output reconstructed image when ran. I have saved all the segmented image outputs from both U-net and SegNet in a separate folder ksoundar/Proj/Result. The code will printout IOU score and precision values for all 20 images. I have documented the results in my Report, please take a look at the images. I have included the references as comments in the code

4. The Results folder contains ROC curves  and predicted images in separate folders for visualization 


It was a great learning experience. 

Thank you
Krishna
