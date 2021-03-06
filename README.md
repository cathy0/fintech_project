

### 3分鐘影片

[![](3min影片.PNG)](https://www.youtube.com/embed/GyuDfw4FKzg)

### 15分鐘影片

[![](15min影片.PNG)](https://youtu.be/9TEgCBaxdiM)

### 簡報
[簡報](AI挑選最佳基金.pdf)

### 策略選擇excel檔
[策略選擇excel檔](FinalResult.xlsx)

# 永豐金控-AI挑選最佳基金
- [專案概要](#專案概要)
  - [問題介紹](#問題介紹)
  - [主要方法](#主要方法)
- [挑選基金的策略](#挑選基金的策略)
  - [傳統法則](#傳統法則)
  - [機器學習](#機器學習)

# 專案概要
## 問題介紹 
當面臨投資時，很多人不知道該從何下手、毫無頭緒，因而有4433等篩選基金的法則，但這些方法未經證實且複雜。
隨著科技的發達與人工智慧的出現使人們對於投資有更多不同的選擇，因此我們希望能透過人工智慧的方式，在過往的資料當中找出規律，並且為所有的投資人找出一個最理想的基金。


## 主要方法 
我們先將基金分成了十二個類別，例如：科技型基金、股債混合型基金等等，再用各種不同的傳統策略以及演算法模型，在每一個類別都挑選出績效最好的一個方法，並且與該類別的所有基金之平均績效進行比較。


>[回目錄](#永豐金控-AI挑選最佳基金)

# 挑選基金的策略
## 傳統法則
依據基金過去的表現，挑選預期未來有潛力的基金，我們使用兩個Rule-based策略，分別是4433法則及3163法則。依據法則挑選符合條件的基金後，再選取sharpe ratio最高的五檔基金。


<div align=center><img width="70%" src="https://github.com/cathy0/fintech_project/blob/main/4433.png" alt="傳統法則-4433法則 示意圖"/></div>

<div align=center><img width="70%" src="https://github.com/cathy0/fintech_project/blob/main/3163.png" alt="傳統法則-3163法則 示意圖"/></div>
  

## 機器學習
利用處理後的淨值資料計算報酬率後，計算出13個特徵值，將特徵值進行特徵工程。模型所使用的特徵工程為PCA主成份分析及StandardScaler標準化，讓模型較不容易發生過度配適的情形。再將特徵值丟入監督式學習的模型中訓練，並使用模型預測基金報酬率並選出未來報酬率最高的五檔基金。


<div align=center><img width="70%" src="https://github.com/cathy0/fintech_project/blob/main/ml.png" alt="機器學習 示意圖"/></div>

>[回目錄](#永豐金控-AI挑選最佳基金)

