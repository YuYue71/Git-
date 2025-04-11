## 在開始使用 Git 之前，建議先設定使用者資訊，這些資訊會附加到每次提交中，方便追蹤修改的來源。

```bash
# 設定全域的使用者名稱，讓 Git 知道提交是由誰執行的
git config --global user.name "你的名稱"

# 設定全域的電子郵件地址，通常使用與 GitHub 帳戶相關聯的 Email，便於身份驗證和追蹤
git config --global user.email "你的Email"

# 設定初始化 Git 倉庫時的預設分支名稱為 main，現代專案通常使用 main 而非舊版的 master
git config --global init.defaultBranch main

# 設定 VSCode 作為 Git 的預設文字編輯器，--wait 參數確保編輯完成後才返回 Git
git config --global core.editor "code --wait"
```