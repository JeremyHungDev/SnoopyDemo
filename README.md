# Snoopy Demo

一個以 Nginx 為基礎的單一服務 Docker 靜態網站，展示 Snoopy 相關內容。

## 特點

- 單一容器，無外部依賴
- 三行 Dockerfile
- `docker run` 直接啟動

## Build & Run

```bash
cd site
docker build -t snoopy:local .
docker run -p 8080:80 snoopy:local
```

瀏覽器開啟 [http://localhost:8080](http://localhost:8080)

## 與 TodoDockerDemo 對比

| | TodoDockerDemo | SnoopyDemo |
|---|---|---|
| 服務數量 | 2（API + PostgreSQL） | 1 |
| Dockerfile 階段 | 多階段 | 單階段 |
| 外部依賴 | PostgreSQL（執行時） | 無 |
