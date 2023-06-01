# Files and folders in this directory:      
1- readme.md: This file provides information about the submitted files and how to set up the environment for this project.      
2- proposal.pdf: The file already sumbitted as a project propasal.       
3- project_report.pdf: A documentation for the project and its findings.      
4- arvato.ipynb: a jupyter notebook. The code to be assessed.     
5- arvato.html: same as arvato.ipynb but in html format.    
6- azdias_cleaned_numerical.pkl: the main dataset in the unsupervised part after being cleaned.     
7- azdias_pca.pkl: the main dataset after dimentionality reduction using pca.      
8- azdias_pca_cluster.pkl: the main dataset after dimentionality reduction using pca and addition of the column 'cluster' containing the cluster number of each individual.      
9- supervised_predictor: this folder contains the pickled model produced during training 'mailout_train' dataset in the supervised learning part.      

# Setup the environment:     
As autogluon has been used in this project, setting it up is somewhat challenging because it has a lot of dependencies. Therefore, it is recommended to install autogluon firstly on a fresh virtual environment. These are the steps I followed:         
conda activate base    
python --version (AutoGluon requires Python version 3.8, 3.9, or 3.10 and is available on Linux, MacOS, and Windows.)     
python -m venv myenv    
myenv\Scripts\activate     
pip install autogluon     
myenv\Scripts\activate (again)    
pip install ipykernel     
python -m ipykernel install --user --name=myenv --display-name "Autogluon Virtual Environment"    
close jupyter notebook and open again     
pip install pca    
change kernel and choose Autogluon Virtual Environment again    
pip install openpyxl    
