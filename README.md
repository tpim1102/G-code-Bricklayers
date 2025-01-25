#Bricklayers G-code-Z-Shift
Directly process the Bricklayers of G-code to achieve compatibility with slicer software


This script has been enhanced based on the original work by TengerTechnologies available at https://github.com/TengerTechnologies/Bricklayers.


Features
- Directly process the Z-shift of G-code to achieve compatibility with slicer software.
- Adjustable layer height and extrusion multiplier.
- Real-time progress tracking and logging.
- User-friendly GUI with pause and stop functionalities.
![image](https://github.com/user-attachments/assets/fa805df5-5be2-4352-95b7-0648739013cd)

![image](https://github.com/user-attachments/assets/1d63e0f0-392b-4df4-998f-7f6326d7f15b)
![image](https://github.com/user-attachments/assets/1c0a9249-b0e8-4b71-8ac6-fa3d6ea8ef74)

Key Features
G-code File Selection and Import

Browse Button: Users can select the G-code file they wish to process by clicking the "Browse" button. Supported file formats include .gcode, .gc, and .txt.
File Path Display: The selected file's path is displayed in an input field for user confirmation.
Parameter Adjustment

Layer Height Adjustment: A slider allows users to set the desired layer height, ranging from 0.05mm to 1.0mm with 0.01mm increments. Adjusting the layer height can significantly impact the print's detail and speed.
Extrusion Multiplier Adjustment: Another slider enables users to modify the extrusion multiplier, ranging from 0.5x to 2.0x with 0.01x increments. This adjustment affects the amount of material extruded, influencing the print's strength and material consumption.
Processing Controls

Start Processing: Initiates the G-code processing in a background thread, ensuring the GUI remains responsive. The processing involves adjusting the Z-axis movements and extrusion values based on the user-defined parameters.
Pause: Allows users to temporarily halt the processing. This is useful for making intermediate adjustments or addressing unforeseen issues without stopping the entire process.
Continue: Resumes processing after a pause, enabling users to seamlessly continue their tasks.
Stop: Completely terminates the processing. This action disables all control buttons and resets the elapsed time display, ensuring no residual processes continue in the background.
Progress and Time Tracking

Progress Bar: Visually represents the completion status of the processing task, giving users a clear indication of how much work has been done and how much remains.
Elapsed Time Display: Shows the total time elapsed since the start of the processing, formatted as HH:MM:SS. This helps users monitor the duration of their tasks.
Logging

Processing Log Area: A scrollable text area displays real-time logs of the processing steps, including layer detection, block modifications, and any warnings or errors encountered.
Log File: All logs are also saved to a z_shift_log.txt file in the script's directory, providing a persistent record for future reference or troubleshooting.
Export Modified G-code

Export Button: After processing, users can save the modified G-code to a new file by clicking the "Export" button. The tool suggests a default filename based on the original file but allows users to specify a different name or location.



Here is a video about the script.[![54654](https://github.com/user-attachments/assets/06165c32-21a5-426c-bedb-09aaedc62dae)](https://www.youtube.com/watch?v=3RTSSLVJbAs)
https://youtu.be/3RTSSLVJbAs
