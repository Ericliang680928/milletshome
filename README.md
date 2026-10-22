# 米樂家食材 官網（milletshome）

網址：https://ericliang680928.github.io/milletshome/

```
/                     首頁（企業入口）
/products/            線上商店（產品總覽）
/products/manfu-chili-sauce/   滿福果仁辣醬 一頁式購物頁（含購物車、下單、查詢訂單）
/order/               查詢訂單（跨產品共用，用電話查）
/admin/               購物車後台（訂單、商品上架、設定；需通關碼）
/config.js            資料庫連線（Supabase 專案 imc-miaoli-bot，mf_ 資料表）
/db/                  資料庫建置 SQL（備查）
/assets/logo.png      米樂家 logo
```

## 新增產品
1. 複製 `products/manfu-chili-sauce/` 成新資料夾（英文小寫、用 `-` 連字），改內容與照片；
2. 在 `products/index.html` 與根目錄 `index.html` 的 `PRODUCTS` 各加一筆；
3. 後台「商品上架」新增該商品（照片路徑相對於該產品頁，例如 `assets/img/xxx.jpg`）。
   目前後台縮圖以 `admin/index.html` 內的 `PRODUCT_BASE` 解析相對路徑；第二個產品上架時改成用圖片網址或根目錄路徑（`/milletshome/products/…`）即可。

## 舊網址
`one-page/millethome/` 已改為自動轉址到新的產品頁。
