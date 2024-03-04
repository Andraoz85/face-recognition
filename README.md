# Face Recognition Models Comparison
This repository hosts a comparison between two prominent open-source models for face recognition: Dlib's HOG (Histogram of Oriented Gradients) with SVM (Support Vector Machine) and OpenCV with Haar-Cascade classifier, alongside a comprehensive guide on how to implement these models using your own image dataset.

## Mounting Your Drive in Google Colab  
To access your image dataset stored in Google Drive, mount your drive using:
```
from google.colab import drive
drive.mount('/content/drive', force_remount=True)
```

## Processing Your Image Dataset  
To process multiple images stored in a directory:  
```
# Define the path to your image directory on Google Drive
image_directory = '/content/drive/My Drive/images/'

# Process all images in the directory
process_images_in_directory(image_directory, hog_face_detector)
```

## Performance Metrics  
To evaluate the model, calculate the precision, recall, and F1 score using the calculate_performance_metrics function:  
```
# Define your True Positives, False Positives, and False Negatives
TP = # true positives count
FP = # false positives count
FN = # false negatives count

# Calculate performance metrics
Precision, Recall, F1_Score = calculate_performance_metrics(TP, FP, FN)
```
Replace # true positives count, # false positives count, and # false negatives count with the actual counts from your model's performance.

## Visualization of Metrics
The repository includes a script to visualize the calculated metrics as a bar chart:  
```
# This will display a bar chart of Precision, Recall, and F1 Score
plt.show()
```

## License  
The project is open-source and available under the MIT License as found in the LICENSE.md file.
