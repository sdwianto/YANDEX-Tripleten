## Computer Vision to determine a person's age from a photo
#### <i>Sprint focus: Computer Vision, Neural Network, Keras Library, Fully Connected Network, Convolution, LeNet Architecture, Adam Algorithm, ResNet Architecture </i>

Summary:
Project Description: A supermarket franchise called Good Seed wants to explore whether Data Science can help them comply with the law by ensuring that they do not sell age-restricted products to underage customers. They have cameras installed in the cashier area that display a signal when someone purchases age-restricted products. Computer vision methods can be used to determine a person's age from a photo. The task is to build and evaluate a model to verify a person's age based on the provided photos.

EDA Findings:
-	The image dataset contains 7,591 photos with age labels.
-	The average age of the people in the dataset is 29 years.
-	The dataset is predominantly composed of the 15-40 age group.
-	There are only a few photos of older age groups (above 60 years), which may result in the model not training well for this age group and potentially leading to higher prediction errors.
-	Further analysis can be conducted based on different age groups, such as children, adults, and the elderly.
-	The facial sizes in the photos vary, and resizing adjustments may be necessary.

-	Almost all photos have the correct orientation, with horizontal flip being the only applicable augmentation for this dataset.
-	The photo dataset contains images with varying qualities, including black and white and colored photos.

Modeling Analysis:
-	The applied model uses the ResNet50 architecture, the Adam optimizer with a learning rate of 0.0005, relu activation, 20 epochs, and a batch size of 16.
-	The model can predict with an accuracy of MAE (Mean Absolute Error) of 5.117.

Conclusion: The model can perform photo predictions from the provided dataset with high accuracy.
