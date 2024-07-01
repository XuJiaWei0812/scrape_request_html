# scrape_request_html

這是一個使用 Python 爬取電影資料的專案，用於練習 requests 爬取靜態網頁的方法。

## 功能介紹

- 爬取 https://ssr1.scrape.center/ 網站的電影資料
- 解析HTML頁面，提取電影詳細資訊
- 將爬取的資料保存到 `Excel` 檔案中

## 使用套件

- `requests` : 用於發送 HTTP 請求
- `fake_useragent` : 生成隨機 User-Agent
- `BeautifulSoup` : 解析 HTML
- `openpyxl` : 操作 Excel 檔案

## 如何使用

1. 安裝必要的套件:
   
   ```bash
   pip install requests fake_useragent beautifulsoup4 openpyxl
   ```
2. 運行腳本:
   
   ```bash
   python scrape_requests_html.py
   ```
3. 自動爬取網站的所有頁面，並將結果保存在 `scrape_reques_html.xlsx` 文件中。

## 注意事項

- 本腳本僅供學習和研究使用
- 請遵守網站的 `robots.txt` 規則和使用條款
- 爬取過程中設有隨機延遲,以避免對目標網站造成過大壓力
