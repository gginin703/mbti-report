MBTI 功能分析報告 PWA

檔案
  index.html            主程式（跟 Artifact 版內容相同，另外會記住上次選的類型）
  manifest.webmanifest  App 名稱、圖示、顯示方式
  sw.js                 Service Worker，讓 App 可以離線使用
  icons/                App 圖示

在電腦上試
  在這個資料夾開終端機，執行： python -m http.server 8080
  瀏覽器開 http://localhost:8080

放到手機
  PWA 一定要用 HTTPS 網址。把整個資料夾上傳到任一個靜態網站服務：
  - Netlify Drop：開 https://app.netlify.com/drop ，把資料夾拖進去
  - GitHub Pages：建一個 repo，上傳這些檔案，到 Settings > Pages 開啟
  手機開那個網址後：
  - iPhone（Safari）：分享 > 加入主畫面
  - Android（Chrome）：選單 > 安裝應用程式 / 加到主畫面

更新內容後
  把 sw.js 裡的 VERSION 改一下（例如 mbti-v2），手機才會換成新版。
