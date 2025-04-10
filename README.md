# Denoise
# Author : Muralidharan Mani 
# Affiliation : University of Wisconsin-Madison
DenoiseimageMatlab
this MATLAB code and guide you through using it step-by-step.

1. Save the Code as a MATLAB Function:

Open MATLAB.
Create a new script (File > New > Script).
Copy and paste the entire code into the script.
Save the script as DenoiseGUI.m. Make sure the filename matches the function name (DenoiseGUI).
2. Run the Function:

In the MATLAB command window, simply type:
Matlab

DenoiseGUI
Press Enter. This will launch the graphical user interface (GUI).
3. Understanding the GUI:

Multiframe Window Slider:
This slider controls the size of the window used in the wiener2 denoising function.
The value displayed next to the slider shows the current window size.
Adjust the slider to change the window size. Larger values might result in smoother images but could also blur fine details.
Load Image Button:
Click this button to select a TIFF image file (.tif or .tiff).
The selected image will be loaded and displayed in the left axes (labeled "Original Image").
Batch Process Button:
Click this button to select a folder containing multiple TIFF image files.
The code will process each image in the folder, denoise it, and save the denoised images back to the same folder.
Start Button:
After loading an image, click this button to start the denoising process.
The denoise process uses a wiener filter.
A progress bar will appear to show the denoising progress.
The denoised image will be displayed in the right axes (labeled "Denoised Image").
Save Button:
Click this button to save the denoised image(s) to a TIFF file.
Previous Frame (<) and Next Frame (>) Buttons:
If you load a multi-frame TIFF image, use these buttons to navigate between frames.
The current frame number is implicitly tracked, and the original and denoised images will update accordingly.
Original Image Axes (Left):
Displays the original loaded image or the current frame of a multi-frame image.
Denoised Image Axes (Right):
Displays the denoised image or the current denoised frame.
Progress Bar:
Appears when the start button is pressed to indicate the progress of the denoise function.
4. Step-by-Step Usage:

Load an Image:
Click the "Load Image" button.
Navigate to and select your TIFF image file.
The image will appear in the "Original Image" axes.
Adjust the Multiframe Window:
Use the slider to set the desired window size for the denoising algorithm.
The number near the slider will display the current value.
Start Denoising:
Click the "Start" button.
Wait for the denoising process to complete. The progress bar will indicate the status.
The denoised image will appear in the "Denoised Image" axes.
Save the Denoised Image:
Click the "Save" button.
Choose a filename and location to save the denoised image.
Navigate Frames (if applicable):
If you loaded a multi-frame tiff, use the "<" and ">" buttons to navigate between frames.
The images in both axes will update.
Batch Processing (Optional):
Click the "Batch Process" button.
Select the folder containing the TIFF images you want to denoise.
The code will process each image in the folder and save the denoised versions.
Close the GUI:
Close the figure window when you are finished.
Important Notes:

Dependencies: This code relies on the MATLAB Image Processing Toolbox for the wiener2 function. Ensure you have this toolbox installed.
File Permissions: Make sure MATLAB has the necessary read/write permissions for the files and folders you are working with.
Error Handling: The code includes basic error handling (e.g., checking if an image is loaded before denoising).
Memory Usage: If you are working with very large images or a large number of images in batch processing, be mindful of your computer's memory.
This guide should help you effectively use the DenoiseGUI function. If you have any further questions or encounter issues, feel free to ask!
