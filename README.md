# ScientificProgramming2
## Assignment 2 Making multivariate statistics reproducible 

The BRCA1 protein is a tumor suppressor protein which help prevent cells from growing and dividing too fast or in an uncontrolled manner. This protein plays a key role in maintaining the stability of the genetic information of a cell by helping to repair damaged DNA. BRCA1 protein also interacts with many other proteins to regulate the activity of the corresponding genes. Most of the mutations in the BRCA1 gene are associated with an increased risk of breast cancer. Production of a short version of the BRCA1 protein is a consequence of most BRCA1 mutations, which leads to less protein available for repairing damaged DNA.

During this assignment the dataset from the link below will be used, which includes a QHTS Assay to identify small molecule activators of BRCA1 expression (PubChem Assay AID 624202). In this study they wanted to investigate the increase of BRCA1 expression, develop new chemical activator probes and eventually develop a novel prevention or therapeutic agent for breast cancer patients. 
https://pubchem.ncbi.nlm.nih.gov/bioassay/624202#section=Top

This data will be processed, analysed and a visualization of the results will be created. The analysis includes Partial Least Squares (PLS) regression which reduces the number of predictors to obtain a set of components that explains the maximum correlation between the predictors and the response variables. Finding the smallest set of components with the greatest prediction will be done by including cross-validation. The selection of the components is based on the amount of variance explained by the predictors and between the predictors and the responses. The number of components will be less than the number of predictors when the predictors are highly correlated or if a smaller amount of components model the response perfectly. PLS is able to fit multiple response variables in one model. The R package used to perform Partial Least Squares regression is the pls package. 

A R Markdown notebook will be created in RStudio to combine the code of the analysis together with clear documentation to make the code reproducible. The data will be split in a training and test set, the training set to build the Partial Least Squares model and the test set to eventually test the prediction model. The division of the dataset will happen randomly and cross-validation will be applied to estimate the number of latent variables needed for the prediction model. Two types of cross-validation will be tested and compared, Leave-on-Out and Leave-10%-Out. 
The goal of this assignment is to make reproducible code, which allows myself or others to easily reproduce my results or making it easy to adapt slight changes. 

### Prerequisites 

RStudio

#### Programming language

R

#### File format

Markdown

#### Programming Approaches
*	Interactive notebooks
*	Multivariate statistics
