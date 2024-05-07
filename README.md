# Unstructured Data Handling Project

## 1. Introduction

This project focuses on handling unstructured data from drone SRT files using Python. The main objectives are to create a structured dataframe from the SRT data, add additional features such as speed, and augment a video with overlays containing information from the dataframe. The project aims to provide experience in handling unstructured data and integrating it into a visual representation.

This should be the final output
![Figure 1](https://raw.githubusercontent.com/udayaKherath/Unstructured-data-handling/main/OutputVideoFrameExample.png)

## 2. Implementation Details

### 2.1 Data Processing

- **SRT File Parsing:** Python scripts are used to parse the SRT files and extract relevant information such as latitude, longitude, altitude, and timestamp.
- **DataFrame Creation:** The extracted data is structured into a pandas dataframe, which serves as the basis for further analysis and feature engineering.
- **Feature Engineering:** Additional features like distance and speed are calculated based on the extracted data.

### 2.2 Video Augmentation

- **Image Extraction:** Using OpenCV, images are extracted from the video at each timestamp provided in the SRT file.
- **Overlay Generation:** Overlays containing information from the dataframe (such as latitude, longitude, altitude, and speed) are generated and added to each frame of the video.
- **Video Compilation:** The augmented frames are compiled back into a video format, creating a visual representation of the data.


## 3. Usage

1. Ensure Python and the required libraries (such as pandas, OpenCV) are installed.
2. Place the SRT file (`drone_flight.srt`) and the input video (`input_video.mp4`) in the `data/input/` directory.
3. Run the `main.py` script to execute the data processing and video augmentation.
4. The augmented video will be saved in the `data/output/` directory as `augmented_video.mp4`.

## 4. Future Improvements

- Implement additional features and visualizations based on the data extracted from the SRT files.
- Enhance the user interface for better interaction and customization of the augmented video.
- Optimize the code for faster processing and better performance, especially for larger datasets.

## 5. Contribution

Contributions to this project are welcome! If you have ideas for improvements or new features, feel free to fork the repository and submit a pull request.

