# Car Price Predictor :car:


https://user-images.githubusercontent.com/106590141/209450829-59498acf-287f-4f1b-afd5-82ed4bfa8eca.mp4








Reference link : [campusX](https://youtu.be/iRCaMnR_bpA) <br>
[Dataset](https://github.com/rajtilakls2510/car_price_predictor/blob/master/quikr_car.csv)

### OneHotEncoder on categorical features
```
ohe = OneHotEncoder()
ohe.fit(X[['name','company','fuel_type']])
```
Check the categories
```
ohe.categories_
```
To perform OneHotEncoding on x_train and y_train
make_column_transformer
```
column_trans = make_column_transformer((OneHotEncoder(categories = ohe.categories_),['name','company','fuel_type']),
                                        remainder= 'passthrough')
```
### make pipeline:
```
model = LinearRegression()
```
```
pipe= make_pipeline(column_trans,model)
```
- This pipe line will first apply columns transformer
- In columns_trans first this will apply OneHotEncoder
- Then these columns ['name','company','fuel_type'] will transform 
- After that it will send the all data to linear regression model

```
pipe.fit(x_train,y_train)
```






