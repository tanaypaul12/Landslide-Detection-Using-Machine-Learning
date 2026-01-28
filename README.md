# Landslide-Detection-Using-Machine-Learning (Random Forest)
Landslide Prediction Project
This project focuses on landslide susceptibility prediction using geospatial data and machine learning techniques. The objective is to identify areas prone to landslides by learning patterns from past landslide events and relevant conditioning factors.




Data Preparation

Landslide Inventory
Historical landslide event locations were collected and used as the primary reference dataset, lebeled 0 as non landslide point which is inventory points and 1 as Landlide points  

Factor-Level Data Extraction
For each landslide location, point-wise values of conditioning factors were extracted. These factors typically include:

1.Slope

2.Elevation

3.Aspect

4.Distance to roads

5.Distance to rivers

6.Rainfall

7.Topographic Wetness Index (TWI)

8.Curvature

Non-Landslide (Random) Points
Random points were generated in landslide-free areas to represent non-landslide conditions. The same factor-level data were extracted for these points to create a balanced dataset.
<img width="931" height="183" alt="image" src="https://github.com/user-attachments/assets/010a0f4e-96c2-4f0c-a23c-10a018d008c7" />



**Model Development**

The combined dataset (landslide and non-landslide points) was divided into training and testing datasets.

A Random Forest classifier was used for landslide susceptibility modeling due to its robustness in handling nonlinear relationships and multicollinearity among factors.

The model learns the relationship between past landslide occurrences and conditioning factors to predict landslide probability.

**Model Evaluation**

The trained model was tested using independent random points.

Performance was evaluated using standard classification metrics such as:

<img width="2431" height="3205" alt="landslide_susceptibility_map_final (1)" src="https://github.com/user-attachments/assets/8ac828a4-41bb-434f-a29d-952987421544" />

<img width="2431" height="3205" alt="landslide_susceptibility_map_final" src="https://github.com/user-attachments/assets/faa1fb76-6e47-4648-a50e-3a60797e198f" />

**Accuracy**

Precision
ROC–AUC
Output

<img width="578" height="455" alt="image" src="https://github.com/user-attachments/assets/98783ec9-7423-4df9-a75d-bb71acc6bab6" />

The final output is a landslide susceptibility map, categorizing areas into different risk levels (e.g., low, moderate, high, very high).

The model can support disaster risk reduction, land-use planning, and early warning systems.

**Tools & Technologies**

GIS for spatial data processing and factor extraction

Python for data analysis and modeling

Scikit-learn for Random Forest implementation
