# 檢查Git的版本
git --version

# 設定作者資料
## 設定作者姓名
git config --global user.name "name"

## 設定作者電子郵件
git config --global user.email "email@email.com"

# 初始化建立Git儲存庫
git init

# 檢查當前目錄中所有檔案狀態
git status

# 追蹤檔案
## 追蹤指定檔案
git add 檔案名.副檔名

## 追蹤所有同樣副檔名的檔案
git add *.副檔名

## 追蹤當前目錄所有檔案
git add .

# 建立還原點
git commit -m "還原點註解"

# 列出歷史還原點內容  按Q視退出檢
git log

## 列出歷史還原點內容簡化版  按Q視退出檢
git log --oneline

# 比較還原點差異  還原點ID可在歷史內容中檢視
git diff 還原點ID -- 檔案名.副檔名

# 還原指定文件
git checkout 還原點ID -- 檔案名.副檔名

# 還原所有文件    此操作不可逆
git reset --hard 還原點ID

# 指定忽略追蹤檔案
建立一個檔名為.gitignore的檔案
隨後在此檔案中輸入要忽略的檔案名稱與副檔名
例如:PQ.py , *.txt , *.png 等等


# GitHub相關指令
## 初始推送與連接本地與GitHub儲存庫
git remote add origin 儲存庫網址
git branch -M main
git push -u origin main

## 本地檔案推送到GitHub上
git push

## 載入協作者Code檔案
git clone 協作專案網址

## 即時載入GitHub檔案
git pull

## 分支工作環境
# 建立分支
git checkout -b 分支名稱

# 初始推送分支檔案到GitHub  第一次使用後都可直接用git push
git push origin 分支名稱