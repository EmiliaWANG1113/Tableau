# Tableau-absoluteposition
利用X & Y 絕對位置進行視覺化排版
使用物聯網pm2.5濃度資料疊合在地圖上(利用對應的device id打在地圖上)

#### 選定感測點
因感測點位需每顆逐一判斷XY位置，所以先挑選4顆感測器為主

<img width="600" height="350" src="https://github.com/EvelynWANG1113/Tableau-absoluteposition/blob/main/%E9%81%B8%E5%AE%9A%E6%84%9F%E6%B8%AC%E9%BB%9E.png"/>

#### XY軸座標圖地圖
1. 接著載入四個點的座標資料csv檔，並設定 join 欄位
2. 載入csv後建立join載入背景 XY 圖片
3. 判斷座標對應位置
4. Join 感測器與 XY 座標軸資料

<img width="600" height="350" src="https://github.com/EvelynWANG1113/Tableau-absoluteposition/blob/main/XY%E8%BB%B8%E5%BA%A7%E6%A8%99%E5%9C%96%E5%9C%B0%E5%9C%96.png"/>


## Link
[https://public.tableau.com/app/profile/evelyn1382/viz/absoluteposition/XY?publish=yes](https://public.tableau.com/app/profile/evelyn1382/viz/absoluteposition/XY?publish=yes)
