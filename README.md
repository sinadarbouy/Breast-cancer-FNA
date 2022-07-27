# Breast-cancer-FNA
## Diagnostic Systems
Diagnostic systems are frequently used in medicine to classify X-ray images, predict the risk of mortality, etc. 
In this project, a classic database concerning breast cancer diagnosis is studied to investigate model interpretability.

## Implementation
* The file wdbc.pkl contains a dataset of patients tested for breast cancer using a fine needle aspirate (FNA). Each patient is represented by statistics of 10 different features of multiple cell samples, as well as a diagnosis (malignant or benign). The file has columns in the order: subject id, label features.
* Identification of breast cancer from FNA is based on several factors that make tumor cells stand out among regular tissue. 
* These factors are summarized as follows: The size of cells tends to be homogeneous given a specific type of tissue.
	1) The presence of significantly large cells is evident in the uncontrolled growth that is indicative of malignant tumors.
	2) The shape of benign cells usually shows only limited variance, whereas malignant cells can develop arbitrary structures that do not conform with the general pattern of their surroundings.
	3) The color of the cell nucleus should be identical to regular cells of the same type. Cancer cells often have significantly large and darker nuclei that are more densely packed with DNA
	4) Regular cells show a similar texture. Malignant tumors, on the other hand, can range from smooth surfaces to ragged or lumpy textures for neighboring cells.
	5) Finally, for healthy tissue, cell arrangement tends to be orderly, with regular distances between cells. Cancer cells can spread out or clutter almost arbitrarily
* This project implements and evaluates the following classifiers in the task of assigning the diagnosis of malignant or benign.
	1) A rule-based classifier
	2) A random forest classifier using the sklearn framework applied to the features given in the supplied database.
	3) A classifier of our design that attempts to trade off interpretability and classification performance.
