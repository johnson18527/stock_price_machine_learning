# 案例練習：股價預測
## 問題定義
於監督式回歸框架中，預測微軟股票的周報酬率，找出影響微軟股價因素
### 輸入變數
微軟周報酬率、IBM周報酬率、Google周報酬率、美元/日圓、英鎊/美元、標準普爾500指數、道瓊指數、波動指數

## 資料說明
### 備註：本案報酬計算階以5個交易日(T+5收盤減T日收盤 or T收盤減T-5日收盤)為單位
![image](https://github.com/johnson18527/stock_price_machine_learning/blob/main/pic/%E8%9E%A2%E5%B9%95%E6%93%B7%E5%8F%96%E7%95%AB%E9%9D%A2%202023-12-27%20203056.png)

## 資料轉換
 - 正規化(np.log())
 - 資料整理(dataframe.loc、dataframe.iloc、pd.concat()、pd.dropna()、np.diff()、np.shift())
## 探索性資料分析
 - 敘述性統計(dataframe.head()、dataframe.describe())
 - 長條圖(dataframe.hist())
 - 機率密度圖(dataframe.plot()) 
 - 熱力圖(dataset.corr()、sns.heatmap)
 - 散點圖(scatter_matrix())
 - 時間序列(sm.tsa.seasonal_decompose())
## 模型比較
 - LinearRegression 
 - Lasso 
 - ElasticNet 
 - KNeighborsRegressor
 - DecisionTreeRegressor 
 - SVR ．MLPRegressor 
 - AdaBoostRegressor
 - GradientBoostingRegressor 
 - RandomForestRegressor
 - ExtraTreesRegressor
 - ARIMA
## 模型評估
 - 交叉驗證(KFold()、neg_mean_squared_error)
 - MSE(mean_squared_error)
 - 視覺化(pyplot.boxplot()、pyplot.bar())
## 其他參考工具
 - Feature Selection(SelectKBest)
## 參考書籍
 - 《金融機器學習與資料科學藍圖》