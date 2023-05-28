# Tableau-pm2.5
使用環保署空氣品質IOT物聯網資料與空氣品質國家測站資料進行data join、union、blend
Data來源： [https://ci.taiwan.gov.tw/dsp/environmenta](https://ci.taiwan.gov.tw/dsp/environmenta)
 
### PM2.5濃度地圖(2/1-2/5)
1. 將2020/02/01-2020/02/05 5天Iot資料進行union，再join點位資料EPAIot_station.csv(join device id欄位)
2. 每個點位意思(顏色越紅代表濃度較大)

<img width="650" height="400" src="https://github.com/EvelynWANG1113/Tableau-pm2.5/blob/main/PM2.5%E6%BF%83%E5%BA%A6%E5%9C%B0%E5%9C%96(2%3A1-2%3A5).png"/>

### 感測器與國家測站pm2.5變化線圖(2/1-2/5)
1. 進行資料混合(data blend)，混合兩個不一樣的資料集(EPA_OD_202002.csv與eap_micro_20200201.csv)
2. 利用時間欄位進行混合個分別為：

   國家測站(EPA_OD_202002.csv) -> TIME(需增加計算欄位，減一小時)
   
   IOT感測器(eap_micro_20200201.csv) -> Publishtime(以分鐘為單位，需增加計算欄位)

<img width="650" height="400" src="https://github.com/EvelynWANG1113/Tableau-pm2.5/blob/main/%E6%84%9F%E6%B8%AC%E5%99%A8%E8%88%87%E5%9C%8B%E5%AE%B6%E6%B8%AC%E7%AB%99pm2.5%E8%AE%8A%E5%8C%96%E7%B7%9A%E5%9C%96(2%3A1-2%3A5).png"/>

## Link
[https://public.tableau.com/app/profile/evelyn1382/viz/_16836494093160/sheet1](https://public.tableau.com/app/profile/evelyn1382/viz/pm2_5_16837967181580/PM2_521-25?publish=yes)
