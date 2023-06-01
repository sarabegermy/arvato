# Files and folders in this directory:      
1- readme.md: This file provides information about the submitted files and how to set up the environment for this project.      
2- proposal.pdf: The file already sumbitted as a project propasal.       
3- project_report.pdf: A documentation for the project and its findings.      
4- arvato.ipynb: a jupyter notebook. The code to be assessed.     
5- arvato.html: same as arvato.ipynb but in html format.    

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
