# Traffic Sign Detection Using AI Research 

This repository contains all the Traffic Sign Detection Using AI research I have done through the Project Engineering Success research program by the San Jose State Engineering department.

## Inference Video 

You can view the inference video that my model annotated at this link: https://drive.google.com/file/d/1JEZqolQYS4HieL6bMvFAzoruH8MMTtWq/view?usp=sharing

This video was annotated by the model trained on the GTSDB dataset using YOLOv8.

## An Overview of My Research Work

I was mentored by Professor Birsen Sirkeci from the College of Engineering at San Jose State University. This research work was done through the Project Engineering Success Research Program at SJSU.

### Traffic Sign Classification Research

The first semester of my research work consisted of training a machine learning model to classify German traffic signs. I trained my model on the German Traffic Sign Recognition Benchmark (GTSRB) dataset. I used Python, TensorFlow, Keras, and scikit-learn to train my model. I used 80% of the images for training, and 20% of the images for testing my model. I trained my model using Google Colab. 

My model was able to classify most of the images correctly, achieving an accuracy of about 99%. Some images were incorrectly classified, but those images were often too blurry or pixelated to clearly make out what kind of traffic sign it was.

You can [click here](German_Traffic_Signs_Image_Classification/GTSRB_Image_Classification.ipynb) to view my model's source code and results. 

### Traffic Sign Detection Research

The second semester of my research work consisted of training a machine learning model detecting traffic signs in a video using YOLOv8. I trained my model on the German Traffic Sign Detection Benchmark (GTSDB) dataset. To use YOLOv8 to detect objects in a video, the model needs to have a dataset of images with boundary boxes around objects of interest, which in my case, were traffic signs. The GTSDB dataset on Roboflow contained these boundary boxes which allowed me to use the dataset with YOLOv8.   

After I trained my model, I ran an inference on a video I found on YouTube of a person driving in Germany. The model I trained was able to identify the traffic signs it was trained on with high accuracy. Sometimes, my model would incorrectly classify a particular traffic sign, but would quickly correct itself as it got closer to the traffic sign in the video. Some traffic signs and signals lights are not detected because they are absent in the GTSDB dataset, and therefore, my model was not trained on those traffic signs.

You can [click here](German_Traffic_Sign_Object_Detection/GTSDB_Traffic_Sign_Detection_Using_YOLOv8.ipynb) to view my model's source code.

You can [click here](https://drive.google.com/file/d/1JEZqolQYS4HieL6bMvFAzoruH8MMTtWq/view?usp=sharing) to view the annotated video my model generated.

You can [click here](https://www.youtube.com/watch?v=QfnkMGgvFGs) to view the original video I found on YouTube of a person driving in Germany.

# Tools and Technologies Used 

* Python 3
* YOLOv8
* TensorFlow
* Keras
    * Sequential Model
* scikit-learn
    * confusion_matrix
    * classification_report
    * train_test_split
* NumPy
    * NumPy arrays
* Matplotlib
    * Histogram
* Google Colab
* Roboflow
