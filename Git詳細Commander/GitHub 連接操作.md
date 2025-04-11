## 完成本地版本控制後推送到 GitHub 進行遠端管理或分享

```bash
# 綁定遠端倉庫，<URL> 替換為 GitHub 專案的 URL
git remote add origin <URL>

# 檢查遠端倉庫連結是否正確
git remote -v

# 推送當前分支（預設 main）到遠端並設為預設追蹤分支
git push -u origin main

# 後續提交直接推送更新到遠端
git push

# 拉取遠端最新版本並合併，避免衝突
git pull
```

# 注意：
## 如果使用 SSH 方式連接 GitHub，需要先在本地產生金鑰，並將金鑰內容複製到 GitHub 帳戶的 SSH Keys 設定中。

```bash
# 生成 SSH 金鑰，-t 指定密鑰類型（這裡使用 ed25519 為較安全的選擇），-C 則用來備註 Email 資訊
ssh-keygen -t ed25519 -C "your_email@example.com"
# 完成後，將 ~/.ssh/id_ed25519.pub 檔案中的內容貼到 GitHub 的 SSH Keys 頁面
```