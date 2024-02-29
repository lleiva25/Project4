# Project 4: California Produce Recognition Machine
--------------------------------------------------------------------------------------------------------------
Contributors
--------------------------------------------------------------------------------------------------------------
- Leslie Leiva (@LLeiva25)
- Kimberly Toro (@torok839098)
- Kevin Tian (@kevinxtian1)
- Vanessa Vazquez (@15vvanessa)
- Steve Islava (@steveIslava)
  
--------------------------------------------------------------------------------------------------------------
Background
--------------------------------------------------------------------------------------------------------------
We have been commissioned by an agricultural company to develop an advanced image recognition model aimed at enhancing the automation of crop identification processes before shipping to distributors. Additionally, the model will serve consumers by providing regional information about the produce, facilitating informed purchasing decisions. California was chosen as the subject since it produces over 13% of the nation's agricultural production while also being one of the main states to export plant products internationally. California also has a very unique agricultural economy that can be impacted by water supplies and natural diasters.


--------------------------------------------------------------------------------------------------------------
Presentation Link
--------------------------------------------------------------------------------------------------------------
https://docs.google.com/presentation/d/19Z4kXDz9Ik56LlPy4S7T5XggrluEzmuvpu-NFDcMqBk/edit?usp=drive_link

--------------------------------------------------------------------------------------------------------------
Entity Relationship Diagram
--------------------------------------------------------------------------------------------------------------
![Project4_Entity Relationship Diagram](https://github.com/lleiva25/Project4/assets/140974405/8fbcd8b0-f1b6-4814-bafb-9139dc4a43dd)

--------------------------------------------------------------------------------------------------------------
Machine Learning Design
--------------------------------------------------------------------------------------------------------------
![image](https://github.com/lleiva25/Project4/assets/140974405/751303fa-f330-40d2-9a87-5850ae2e7d62)

--------------------------------------------------------------------------------------------------------------
PreTrained Models Tested
--------------------------------------------------------------------------------------------------------------

| Type  | Machine Learning Model |
| ------------- | ------------- |
| Pre-trained  | Inception  |
| Pre-trained  | Xception  |
| Pre-trained  | MobileNetV3  |
| Pre-trained  | Sequential |

--------------------------------------------------------------------------------------------------------------
Process
--------------------------------------------------------------------------------------------------------------
Cleaning Datasets
  1. Deletion of non-relevant columns.
  2. Convert numeric values into integers.
  3. Renaming columns
  4. Filter the datasets to only have records from 2017-2019.
  5. Remove County IDs with multiple county codes.
  6. Drop N/A and zero values from columns.
     
Merging Datasets
  1. Merge multiple datasets from the same source before merging different datasets
  2. Align datasets by filtering records from 2018.
  3. Delete any entries that have a County ID greater than 58.
      - There are 58 counties in California.
  5. Merge data by 'Year' and 'Counties'.

Python Plots
  1. Group 2018 California Agricultural Data by 'CountyName' to find the 'Production' sum of the top ten counties.
  2. Plot bar graph with labeled axis.

Pre-trained Models
  1. Scroll through the directory to find the images for training.
  2. Load image through the engine.
  3. Resize the image for proper analysis.
  4. Convert the image into a 4-dimensional Tensor.
  5. Preprocess the input image array.
  6. Load model from source maxing at 96MB.
  7. Create predictions of the pre-trained model and produce the actual predictions.
  8. Display image.
  9. Loop through the model for each image.
       
--------------------------------------------------------------------------------------------------------------
Future Implimentations
--------------------------------------------------------------------------------------------------------------
- Accessibility 
- Data Ethics
- Partnerships/Stakeholders
- Adapting the model 
- Raise awareness in the community.

--------------------------------------------------------------------------------------------------------------
Future Implimentations
--------------------------------------------------------------------------------------------------------------
California Department of Conservation
https://data.ca.gov/dataset/california-important-farmland-most-recent

California State Assembly Agriculture Report 2020
https://agri.assembly.ca.gov/sites/agri.assembly.ca.gov/files/The%20Impact%20of%20Wildfires%20on%20California%20Agriculture%20Informational%20Hearing%20Report.pdf

California WildFires (2013-2020)
https://www.kaggle.com/datasets/ananthu017/california-wildfire-incidents-20132020

California Census of Agriculture Summary
https://www.nass.usda.gov/Statistics_by_State/California/Publications/AgComm/index.php

California County Codes
https://notary.cdn.sos.ca.gov/forms/notary-county-codes.pdf


