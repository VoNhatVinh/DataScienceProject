# DataScienceProject
This is the final data science project from Mr. Kien

## 1. Member:
- Võ Nhật Vinh - 1612815

- Nguyễn Ngọc Khải - 1612909

## 2. Topic:
- Real estate price classification on Chotot.com

## 3. Structure:

Folders and files:

### Data: contain data crawled from `Chotot.com`
+ `data-full.csv`: all data
+ `data-full.xlsx`: all data
+ `test.csv`: file test
+ `train.csv`: full train. Split in to 2 files: train1.csv and val.csv
+ `train1.csv`: file train
+ `val.csv`: file validation

### Source code: contain  and processing data, train model.
+ get data: code crawled data from Chotot
+ preprocessing and model: contain file `split_train_test.ipynb` and file `Run.ipynb`

### Report: 
+ midterm.pdf: midterm presentation
+ final.pdf: final presentation

## 4. Build model
### Preprocess:
+ Remove: remove house that price is outlier 
+ Filter: filter nan, nan of numeric columns is 0.0, nan of categorical columns is "Khác".
+ Bins: get price to 2 bins
+ One hot encoding
+ Standard Scale

### Model:
+ LogisticRegression
+ MLPClassifier
+ RandomForest
+ KNearestNeighbors

### Based on result, we choose LogisticRegression and RandomForest to get a best model by try different parameters.
+ Best model: RandomForest with 500 trees. Best accuracy on test: 79.9%

## 5. Slide
[Slide](https://docs.google.com/presentation/d/1pgf8lBspJV1ksI9G-cnYnLVxSn213nCMq72PPqCSL7I/edit#slide=id.p)


## 6. How to run:
- copy file `test.csv`, `train.csv`, `train1.csv`, `val.csv` from folder data to folder source code/preprocessing and model.
- Open file `Run.ipynb` and run.
