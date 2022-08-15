# 介紹
這是Kaggle上的一個競賽，https://www.kaggle.com/competitions/foursquare-location-matching。    

當在未知區域尋找附近的餐館或計劃差事時，期望獲得相關、準確的訊息。Foursquare 擁有 12 年以上完善此類方法的經驗，是全球 POI (points-of-interest) 數據的第一大獨立提供商。為了保持最高水平的準確性，數據必須通過來自多個來源的及時更新進行匹配和刪除重複資料。     

在此比賽中，將匹配 POI。使用包含超過一百萬個 Places 項目的數據集，這些項目經過大量修改以包含雜訊、重複、無關或不正確的信息，目的是生成一種算法來預測哪些 Place 項目代表相同的興趣點。每個 Place 項目都包含名稱、街道地址和坐標等屬性。

# 方法
Haversine距離是一個用來計算兩個經緯度點之間距離的方法   
$a=\sin^2(\frac{\Delta \phi}{2})+\cos (\phi_{1}) \cdot \cos (\phi_{2}) \cdot \sin^2(\frac{\Delta \lambda}{2})$   
$c=2 \cdot \arctan 2(\sqrt{a},\sqrt{1-a})$            
$d=R\cdot c$   
其中 $R=6371$(以公里為單位的地球平均半徑)，$\phi=$緯度，$\lambda=經度$
