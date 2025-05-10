# UCI HAR Dataset Analysis

This project processes and analyzes the UCI Human Activity Recognition (HAR) dataset using R. The dataset contains data collected from smartphone sensors to recognize various human activities.

## Dataset Description

The dataset includes recordings of 30 subjects performing six different activities. It includes data from accelerometers and gyroscopes in three domains: time, frequency, and magnitude.

The activities in the dataset are:
1. Walking
2. Walking Upstairs
3. Walking Downstairs
4. Sitting
5. Standing
6. Laying

## Project Steps

This R script performs the following steps:

1. **Download and Unzip the Dataset**  
   If the dataset is not already present, the script will download it from a URL and unzip the files.

2. **Load and Clean the Data**  
   The script loads the activity labels and features from the dataset, extracts only the mean and standard deviation measurements, and cleans the feature names to be more readable.

3. **Merge and Label the Data**  
   It combines the training and test datasets and applies descriptive activity names to the data.

4. **Generate a Tidy Dataset**  
   A tidy dataset is created, which calculates the average of each variable for each subject and activity.

5. **Save the Tidy Data**  
   Finally, the processed data is written to a text file `tidydata.txt`.

## Requirements

- R (version 3.5 or higher)
- dplyr package (can be installed using `install.packages("dplyr")`)

## How to Run

1. Download the UCI HAR Dataset from the [official UCI repository](https://archive.ics.uci.edu/dataset/240/human+activity+recognition+using+smartphones).
2. Unzip the dataset to a folder named `UCI HAR Dataset`.
3. Save the provided R script (e.g., `process_data.R`) in the same directory as the dataset.
4. Run the script in R or RStudio by executing the following command:

   ```r
   source("process_data.R")
