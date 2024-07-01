# 電影資料爬蟲

這是一個使用Python爬取電影資料的專案,用於練習 requests 爬取靜態網頁的方法。

## 功能

- 爬取 https://ssr1.scrape.center/ 網站的電影資料
- 解析HTML頁面,提取電影詳細資訊
- 將爬取的資料保存到Excel檔案中

## 使用的庫

- `requests` : 用於發送HTTP請求
- `fake_useragent` : 生成隨機User-Agent
- `BeautifulSoup` : 解析HTML
- `openpyxl` : 操作Excel檔案

## 主要功能

1. `get_fetch_html()` : 獲取HTML頁面
2. `parse_list_html()` : 解析列表頁面,提取詳細頁面URL
3. `parse_detail_html()` : 解析詳細頁面,提取電影資訊
4. `write_to_excel()` : 將資料寫入Excel檔案

## 如何使用

1. 安裝必要的庫:
   
   ```bash
   pip install requests fake_useragent beautifulsoup4 openpyxl
   ```
3. 運行腳本:
   
   ```bash
   python scrape_requests_html.py
   ```
5. 自動爬取網站的所有頁面，並將結果保存在 `scrape_reques_html.xlsx` 文件中。

## 注意事項

- 本腳本僅供學習和研究使用
- 請遵守網站的 `robots.txt` 規則和使用條款
- 爬取過程中設有隨機延遲,以避免對目標網站造成過大壓力
