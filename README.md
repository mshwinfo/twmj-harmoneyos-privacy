# 雀翎傳說 隱私聲明

`index.html` 就是整份隱私聲明（繁中＋英文摘要），用 GitHub Pages 對外，商店上架填這個網址：

https://mshwinfo.github.io/twmj-harmoneyos-privacy/

## 開 GitHub Pages（只要做一次）

repo 的 **Settings → Pages → Build and deployment**：Source 選 *Deploy from a branch*，
Branch 選 `main`、資料夾 `/ (root)`，存檔。一兩分鐘後上面的網址就會活。

## 改內容

**不要直接改這裡的 `index.html`**。內容只改主 repo（`mshwinfo/twmj-harmoneyos`）的
`entry/src/main/ets/common/GuideContent.ets`（`PRIVACY_DATE`、`PRIVACY_PARAS`、`PRIVACY_CONTACT`，
鴻蒙版與 Web 版的「玩法說明 → 關於與隱私」與首次開啟的同意視窗都讀它），再在主 repo 跑：

```bash
node tools/gen-privacy-page.mjs      # 產生 docs/store/privacy/index.html（中文一字不差，附英文翻譯）
```

把產生的 `docs/store/privacy/index.html` 複製過來蓋掉這裡的 `index.html` 推上去。主 repo 的
`node tools/verify.mjs` 會檢查那份原稿跟 App 內一致；這裡推上去之後打開網址看生效日對不對。
