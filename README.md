# Number---Plate---Recognition
Abstract

Automatic Number Plate Recognition (ANPR) is an image processing technology which uses number (license) plate to identify the vehicle. The objective is to design an efficient automatic authorized vehicle identification system by using the vehicle number plate. The system is implemented on the entrance for security control of a highly restricted area like military zones or area around top government offices or in tollbooths.  The developed system first detects the vehicle and then captures the vehicle image. Vehicle number plate region is extracted using the image segmentation in an image. Optical character recognition technique is used for the character recognition. The resulting data is then used to compare with the records on a database so as to come up with the specific information like the vehicle’s owner, place of registration, address, etc. The system is implemented and simulated in Matlab, and it performance is tested on real image. It is observed from the experiment that the developed system successfully detects and recognize the vehicle number plate on real images.

# Introduction
Tollbooths in India generally employ a purely visual system of vehicle classification. However this causes a huge loss of revenue to the firms operating the tollbooths due to rampant malpractices and discrepancies. To keep a tab on the operators some tollbooths employ a system using fibre optic sensors to automatically classify a vehicle in the background and tally the results with the manual entries. However this system is expensive complicated and requires high maintenance. We aim to study the various systems that can be used to replace such a system with a cheaper and efficient alternative 

License Plate recognition is one of the techniques used for vehicle identification purposes. The sole intention of this project is to find the most efficient way to recognize the registration information from the digital image (obtained from the camera). This process usually comprises of three steps. First step is the license plate localization, regardless of the license-plate size and orientation. The second step is the segmentation of the characters and last step is the recognition of the characters from the license plate. Thus, this project uncovers the fundamental idea of various algorithms required to accomplish character recognition from the license plate during Template Matching. 

This feature of the algorithm mentioned above helped in achieving faster character recognition of the license plate. This process of character recognition consists of steps like Image processing, Defragmentation, Resizing and Character localization that are required to be performed on the image in order for Template Matching to be done.

# Algorithms Used 
Algorithm for System:
•	Input image from camera
•	Detect the number plate area
•	Convert into greyscale image
•	Convert to binary image
•	Segmentation
•	Character recognition

Input image from camera
•	Capture image
•	Store the image into a file format

Detect the number plate area
•	Fill small holes including numbers of Number plate so that number plate area will be large to isolate from figure.
•	Determine width and height of the image.
•	 Scan each pixel of line counting number of white pixels in the following system.
•	 Use the step no. 3 for both horizontal and vertical direction.
•	Check number of possible areas.
•	Logically AND with binary image obtained at “Convert image into binary”
algorithm.
•	Crop the required area.

Convert image into binary
•	Identify the intensity of the image
•	Convert image to greyscale
•	Calculate appropriate threshold value for the image
•	Convert the image into binary image using the threshold
Segmentation
    Filter the noise level present in the image.
    Clip the plate area in such a way that only numbers of plate area extracted.
    Separate each character from the plate.

Character Recognition
•	Create the template file from the stored template images.
•	Resize image obtained from segmentation to the size of template.
•	Compare each character with the templates.
•	Store the best matched character.

