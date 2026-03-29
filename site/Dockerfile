# 使用官方 Nginx Alpine image 作為 base（輕量，約 40MB）
FROM nginx:alpine

# 將靜態檔案複製到 Nginx 預設的網頁根目錄
COPY . /usr/share/nginx/html

# EXPOSE 宣告容器監聽的 port（說明用，不會自動開放）
EXPOSE 80
