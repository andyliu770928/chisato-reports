# 小千研究報告站

這是給 GitHub Pages 使用的靜態站輸出目錄。

## 本機更新

```bash
bash /Users/aliu/MEGA/openclaw/automation/chisato_reports/scripts/publish_reports_site.sh
```

## 發佈到 GitHub Pages

1. 建立一個新的 GitHub repository
2. 在這個目錄加上 remote
3. `git add . && git commit -m "Publish reports site"`
4. `git push -u origin main`
5. 在 GitHub repository 設定 Pages，來源選 `Deploy from a branch`，分支選 `main`，資料夾選 `/ (root)`
