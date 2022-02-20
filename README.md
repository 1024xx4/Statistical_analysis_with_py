# Python で理解する統計解析の基礎

## 作中の関数

### `np.histogram()`
度数を求める時に使用
######引数:

- bins: 階級数(int)
- range: 最小値と最大値(tuple)
###### Library
NumPy

---

### `np.cumsum()`
累積和の計算に使用

###### Library
NumPy

---
### `plt.hist()`
Histogram を描画する

###### 引数:
- 第１引数: data
- size: Sample size
- bins: 階級値
- range: 最小値と最大値
- density: `True` で相対度数で集計
- rwidth: 棒の太さ

---
### `np.cov()`
共分散を求める。
ただし、返値は、共分散行列（covariance matrix）または、分散共分散行列（variance covariance matrix）と呼ばれる行列
###### 引数：
- ddof(delta degree of freedom): デルタ自由度
###### Library
NumPy

---
### `np.corrcodf()`
相関係数を計算できる。戻り値は相関行列(correlation matrix)
##### Library
NumPy

---
### `.scatter()`
散布図を描画できる

###### 引数
- 第１引数: x軸の Data
- 第２引数: y軸の Data

###### Library
MatPlotLib

---
### `np.polyfit()`
係数β_0 と β_1 を求める

### `np.ploy1d`
β_0+β_1 x を返す

`np.ployfit` と `np.poly_1d` から y= β_0 + β_1x の回帰直線を求める

###### Library
NumPy

---
### `plt.hist2d()`
Heat Map を作る

##### 引数
第1引数: x軸の Data
第2引数: y軸の Data
bins: 階級数(x と y の階級値(int) を格納した list)
range: 最小値と最大値(Tuple) を格納した list)
##### Library
MatPlotLib

---

### `np.random.choice()`
無作為抽出を行なう
##### 引数
第１引数: 抽出する対象の List.
第２引数: Sample size
replace: True: 復元抽出 / False: 非復元抽出
#### Library
NumPy

---
### `np.random.seed()`
発生させる乱数の元となる数字。定義することで毎回同じ乱数を得ることができる。
毎回同じ乱数を得ることができ、Code の再現性を保つことができる

---
### `np.all()`
すべての要素が True のときのみ True を返す。
確率がすべて０以上であるか確認できる。
#### Library
NumPy

---
### `stats.bernoulli()`
ベルヌーイ分布に従う確率変数をつくることができる
###### 返り値
`rv_frozen object` ※ベルヌーイ分布に従う
- rv_frozen.pmf: 確率関数を計算する
- rv_frozen.cdf: 累積密度関数を計算でする
- rv_frozen.mean: 期待値を計算する
- rv_frozen.var: 分散を計算する

####### 引数
p: Parameters 

###### Library
scipy.stats