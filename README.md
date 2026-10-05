# 雀翎傳說 隱私聲明

`index.html` 就是整份隱私聲明（繁中＋英文摘要），用 GitHub Pages 對外，商店上架填這個網址：

https://mshwinfo.github.io/twmj-harmoneyos-privacy/

## 開 GitHub Pages（只要做一次）

repo 的 **Settings → Pages → Build and deployment**：Source 選 *Deploy from a branch*，
Branch 選 `main`、資料夾 `/ (root)`，存檔。一兩分鐘後上面的網址就會活。

## 改內容

App 裡（`雀翎傳說` 的「玩法說明 → 關於與隱私」分頁）有一份一模一樣的文字，
改這裡要一起改那邊（主 repo `entry/src/main/ets/common/GuideContent.ets` 的 `PRIVACY_PARAS`，
鴻蒙版與 Web 版共用那一份），生效日（`PRIVACY_DATE`）也要同步。
