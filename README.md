# SIGCUP2023

## File Info
- [GPKG](https://github.com/zhwang0/SIGCUP2023/tree/main/GPKG): a folder storing the lake_poygons_test.gpkg file, containing polygon outlines of predicted lakes.
- [model_ckp](https://github.com/zhwang0/SIGCUP2023/tree/main/model_ckp): a folder storing the TensorFlow checkpoints of the model (must be put in the same directory of the trian.py file).
- [Train.py](https://github.com/zhwang0/SIGCUP2023/tree/main/Train.py): a Python file predicting the lake outlines.
- [Preprocess.ipynb](https://github.com/zhwang0/SIGCUP2023/tree/main/Preprocess.ipynb): a Python Jupyter Notebook to crop the large satellite image into six regions for training and testing. Recommend crop images when the prediction is slow (See Note 1 for details).

## Library Versions
- numpy version =  1.23.3
- pandas version =  1.4.4
- rasterio version =  1.3.8
- cv2 version =  4.6.0
- geopandas version =  0.14.0
- shapely version =  2.0.1
- tensorflow version =  2.10.0

## Usage
1. 



## Note 
1. The estimated prediction time for all test regions is about 1 hour using an NVIDIA RTX A4500. Since the raw satellite is very large, it is recommended to split the raw image into 6 regions. We have done this process using [Preprocess.ipynb](https://github.com/zhwang0/SIGCUP2023/tree/main/Preprocess.ipynb) and the cropped images are stored in a (Google Drive)[https://drive.google.com/drive/folders/1LlkRJyiL0nsJdSD7HVYVpbizbrC9cUpB?usp=sharing] for your convenience.
2. Other preprocessing and training codes are available upon request.


## Team
1. Zhihao Wang, zhwang1@umd.edu, University of Maryland
2. Yiqun Xie, xie@umd.edu, University of Maryland
3. Xiaowei Jia, xiaowei@pitt.edu, University of Pittsburgh
