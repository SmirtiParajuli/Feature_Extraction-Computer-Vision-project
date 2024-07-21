*******************************Image Segmentation and Feature Extraction GUI***************************************
Overview:

	This project is a graphical user interface (GUI) application designed for image segmentation and feature extraction. The application enables users to load images,
	apply various preprocessing techniques, segment the images using different methods, and extract features using Histogram of Oriented Gradients (HOG). It provides a 
	user-friendly interface for performing these tasks, making it accessible to users without extensive programming knowledge.

Techniques Used:

	-> Grayscale Conversion: Simplifies the image processing by converting the image to grayscale.
	-> Histogram Equalization: Improves the contrast of the image, making features more distinguishable.
	-> Gaussian Blur: Reduces image noise and detail by applying a Gaussian filter.
	-> Hairline Removal: Eliminates thin hairline artifacts from the image for clearer segmentation.

Segmentation Methods:

	->Otsu's Method: An automatic thresholding technique that separates the image into foreground and background.
	->K-means Clustering: Partitions the image into segments based on color or intensity similarities.
	->Canny Edge Detection: Detects edges in the image using a multi-stage algorithm that includes gradient calculation, non-maximum suppression, 
          and edge tracking by hysteresis.

Features: 

	-> Load Image: Load an image from the file system for processing.
	-> Process Image: Apply a series of image processing techniques, including grayscale conversion, histogram equalization, Gaussian blur, and hairline removal.
	-> Segment Image: Segment the processed image using multiple methods, including Otsu's method, K-means clustering, and Canny edge detection.
	-> Display HOG Features: Compute and display HOG features, which are useful for object detection and image analysis.
	-> Save HOG Picture: Save the HOG feature image to the file system for further analysis or documentation.
	-> Evaluate Segmentation: Compare the segmentation results with a ground truth mask and save the best segmentation image. This feature is useful for evaluating the effectiveness of different segmentation methods.
	-> Clear All: Clear all loaded and processed images to start fresh.
	-> Exit: Exit the application.

Usefulness:

          This project is useful for feature extraction in machine learning, as HOG features are widely used in computer vision tasks such as object detection and recognition. The tool allows users to 
          easily extract these features, which can then be utilized in machine learning models for future classification or other processes. Additionally, the application includes functionality for evaluating segmentation 
          methods against a ground truth mask, providing a quantitative measure of performance. This is particularly beneficial in research and development, where comparing different algorithms is crucial.

Installation:

    To run this application, you need to have Python installed along with the following libraries:

	Tkinter
	PIL (Pillow)
	OpenCV
	NumPy
	Scikit-image
	Matplotlib
	Pandas

You can install the required libraries using pip:

      		pip install pillow opencv-python numpy scikit-image matplotlib pandas
Usage:

      Run the Application:use the coode from the Jupyter Notebook file
      Segmentation.ipynb

	Load Image:
		Click on "Load Image" and select an image file to load.
	Process Image:
		Click on "Process Image" to apply grayscale conversion, histogram equalization, Gaussian blur, and hairline removal.
	Segment Image:
		Click on "Segment Image" to segment the processed image using Otsu's method, K-means clustering, and Canny edge detection.
	Display HOG Features:
		Click on "Display HoG Features" to compute and display the HOG features of the processed image.
	Save HOG Picture:
		Click on "Save HoG Picture" to save the HOG feature image.
	Evaluate Segmentation:
		Click on "Evaluate Segmentation" to evaluate the segmentation results against a ground truth mask and save the best segmentation image.
	Clear All:
		Click on "Clear All" to clear all loaded and processed images.
	Exit:
		Click on "Exit" to exit the application.
