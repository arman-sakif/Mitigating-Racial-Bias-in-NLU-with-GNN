# Mitigating-Racial-Bias-in-NLU-with-GNN

This repo currently contains the data pre-processing code implementation. Please click the 'data_cleaning_for_GNN.ipynb' file. 

The code implementation uses google colab and google drive. To use it, you would need to use a gmail account and grant permissions.

//from google.colab import drive
drive.mount('/content/drive')//

above line of code will ask for permission to connect with your google drive. It is because the pre-processed files are saved in google drive. 

The raw dataset is directly accessed from Kaggle using the kagglehub. 
//# Download latest version
path = kagglehub.dataset_download("danofer/compass")
print("Path to dataset files:", path)//

