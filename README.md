# Code for the paper 'Spatial-Spectral Feature Extraction of Hyperspectral Images using Local and Global Side-window Box Filtering' submitted to JSTARS
- Based on YuanhaoGong/SideWindowFilter (https://github.com/YuanhaoGong/SideWindowFilter) open source.
- Adding HSI datasets and some filtering code ( all data were classified using SVM. Some datasets are too large and cannot be uploaded to the GitHub ).

## Parameter:
The data sets and  number of training samples can be selected within the code.  
- DataSetName in {'Indianpines', 'PaviaU', 'XuZhou'}
- classifier in {'raw', 'lgs_box'}
- train_number indicates the number of training samples selected for each category.

## Usage:
For example, when DataSet Indianpines takes 5-30 training sample points for each class, the method of calling lgs_box algorithm for 10 iterations is as follows:
- demo('Indianpines', 'lgs_box', [5,10,15,20,25,30]) 

Then the results are then automatically saved to file "all_result.txt".
