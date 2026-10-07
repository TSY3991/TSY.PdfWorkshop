# PDF 工坊

TSY 微光創作室出品的 Windows 離線 PDF 小工具。所有處理都在你的電腦上完成，檔案不會上傳到任何地方；輸出一律另存新檔，絕不覆蓋原檔。

這個 repo 只放說明與正式發佈檔，下載請到 [Releases](https://github.com/TSY3991/TSY.PdfWorkshop/releases/latest)。

## 功能（17 個工具，分四組）

| 分組 | 工具 |
|---|---|
| 整理頁面 | 整理頁面、擷取頁面、刪除頁面、插入頁面、取代頁面、合併、拆分、頁面對切 |
| 編輯頁面 | 裁剪頁面、加上頁碼、浮水印 |
| 轉換 | 圖片轉 PDF、PDF 轉圖片、PDF 轉 TIFF、PDF 轉文字 |
| 最佳化與安全 | 壓縮檔案、解除密碼 |

## 下載

請到 [最新 Release](https://github.com/TSY3991/TSY.PdfWorkshop/releases/latest) 下載。一般電腦選 x64；Windows on ARM 裝置選 arm64。

| 檔案 | 說明 |
|---|---|
| `PdfWorkshopWin-Setup-vX.Y.Z.exe` | 安裝版（x64） |
| `PdfWorkshopWin-Setup-arm64-vX.Y.Z.exe` | 安裝版（arm64） |
| `PdfWorkshopWin-Portable-x64-vX.Y.Z.zip` | 免安裝版（x64），解壓縮後直接執行 |
| `PdfWorkshopWin-Portable-arm64-vX.Y.Z.zip` | 免安裝版（arm64） |
| `SHA256SUMS-vX.Y.Z.txt` | 各檔案的 SHA-256 雜湊值 |
| `ReadMe.txt`、`LICENSE.txt` | 使用說明與授權聲明 |

也可以從 [微光工具箱](https://tsy3991.github.io/TSY.Microglow-Tools/) 的 PDF 工坊頁面下載。

## 驗證下載檔案

下載後可核對雜湊值，確認檔案沒有損毀或遭竄改。在命令提示字元執行：

```text
certutil -hashfile 檔案路徑 SHA256
```

輸出的值應與 `SHA256SUMS-vX.Y.Z.txt` 內該檔案的值相同。

## 系統需求

- Windows 10 1809（build 17763）以上，或 Windows 11
- x64 或 arm64 處理器
- 不需另外安裝 .NET 或其他執行環境（已內含）

## 第一次執行

本軟體尚未申請程式碼簽章，Windows SmartScreen 可能顯示「Windows 已保護您的電腦」。請點「其他資訊」，再點「仍要執行」。部分防毒軟體可能誤判未簽章的程式元件，處理方式請見隨附的 `ReadMe.txt`。

## 安全承諾

- 永遠不覆蓋原檔：所有輸出一律另存為新檔，檔名自動加後綴，不會與既有檔案重名覆蓋。
- 開啟有密碼的 PDF 時會提示輸入密碼；不提供也不嘗試破解任何密碼。
- 處理大型檔案時會顯示進度，可隨時取消。
- 輸出失敗時會說明原因與下一步。
- 裁剪與對切只是隱藏被裁掉的部分，內容仍留在檔案裡，請勿用來遮蔽機密資料。

## 授權

個人非商業使用，保留一切權利，不開放原始碼。完整條款見每個 Release 附帶的 `LICENSE.txt`。使用的第三方開放原始碼元件（PDFsharp、PDFtoImage、PDFium、SkiaSharp、System.Drawing.Common 等）依各自授權提供，詳見安裝資料夾內的 `THIRD-PARTY-NOTICES.txt`。

## 聯絡方式

授權需求或問題回報，請透過 Facebook 粉絲專頁：[TSY 微光創作室](https://www.facebook.com/TSY.Microglow/)
