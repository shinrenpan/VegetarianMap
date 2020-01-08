台灣蔬食餐廳地圖 (geoJSON)  
不侷限純素餐廳, 有些餐廳可能有葷食.  
歡迎 PR 新增或修正

## 地圖列表
依照英文名字排序

| 區域 | 數量 |
| ----------- | ----------- |
| [全台灣](data/All_City_Map.geojson) |6980|
| [彰化縣](data/Changhua_County_Map.geojson) |396|
| [嘉義市](data/Chiayi_City_Map..geojson) |81|
| [嘉義縣](data/Chiayi_County_Map.geojson) |59|
| [新竹市](data/Hsinchu_City_Map.geojson) |151|
| [新竹縣](data/Hsinchu_County_Map.geojson) |113|
| [花蓮縣](data/Hualien_County_Map.geojson) |108|
| [高雄市](data/Kaohsiung_City_Map.geojson) |770|
| [基隆市](data/Keelung_City_Map.geojson) |62|
| [金門縣](data/Kinmen_County_Map.geojson) |14|
| [連江縣](data/Lienchiang_County_Map.geojson) |4|
| [苗栗縣](data/Miaoli_County_Map.geojson) |95|
| [南投縣](data/Nantou_County_Map.geojson) |216|
| [新北市](data/New_Taipei_City_Map.geojson) |1108|
| [澎湖縣](data/Penghu_County_Map.geojson) |28|
| [屏東縣](data/Pingtung_County_Map.geojson) |236|
| [台中市](data/Taichung_City_Map.geojson) |1191|
| [台南市](data/Tainan_City_Map.geojson) |559|
| [台北市](data/Taipei_City_Map.geojson) |940|
| [台東縣](data/Taitung_County_Map.geojson) |75|
| [桃園市](data/Taoyuan_City_Map.geojson) |420|
| [宜蘭縣](data/Yilan_County_Map.geojson) |206|
| [雲林縣](data/Yunlin_County_Map.geojson) |148|

## 新增修改
請依照 [GeoJSON](https://geojson.org) format 新增一個 **type = Feature**, **geometry.type = Point** 的 Object  
例如:

```javascript
{
  "type": "Feature", // 必填 Feature
  "geometry": {
    "type": "Point", // 必填 Point
    "coordinates": [125.6, 10.1] // Array 放 [經度, 緯度]
  },
  "properties": {
    "name": "我的餐廳", // name 必填
    "address": "台北市內湖區 111 號" // address 必填
    // 可新增其他 Property, 例如 tel
  }
}
```

並放置至各縣市相對應的 geojson 檔案 features array 最後一個. 
