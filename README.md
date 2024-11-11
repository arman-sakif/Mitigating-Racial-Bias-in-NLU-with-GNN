# Mitigating-Racial-Bias-in-NLU-with-GNN

This repo currently contains the data pre-processing code implementation. Please click the 'data_cleaning_for_GNN.ipynb' file. 

The code implementation uses google colab and google drive. To use it, you would need to use a gmail account and grant permissions.

```python
from google.colab import drive
drive.mount('/content/drive')//
```

above line of code will ask for permission to connect with your google drive. It is because the pre-processed files are saved in google drive. 

The raw dataset is directly accessed from Kaggle using the kagglehub. 
```python
# Download latest version
path = kagglehub.dataset_download("danofer/compass")
print("Path to dataset files:", path)//
```

By the end of the code, 3 files will be generated :
1. Filtered recidivism file
2. train_ds
3. test_ds

All three of them goes through label encoding, all attributes are numerical and ready to train models. 

```python
path_recidivism_filtered = '/content/drive/MyDrive/datasets_mine/gnn_dataset/recidivism_filtered.csv'
df.to_csv(path_recidivism_filtered, index=False)

dir_path = '/content/drive/MyDrive/datasets_mine/gnn_dataset/'
train_df.to_csv(dir_path + 'recidivism_train.csv', index=False)
test_df.to_csv(dir_path + 'recidivism_test.csv', index=False)
```
