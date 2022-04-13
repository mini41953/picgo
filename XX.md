# XAMPP 的建置

## 環境條件
- php 7.4.24
- mysql
- xampp-windows

## 建置虛擬主機
1.條件:
  - 主機名稱: web111a
  - 網址: com.tw
  - 網站根目錄: D:\xampp\htdocs\web111a

2.設置步驟:
  - 修改虛擬主機設定檔:`C:\xampp\apache\conf\extra\httpd-vhosts.conf` 如下:

<!-- httpd-vhosts.conf 開啟/最下方 複製 註解拿掉/修改seveer name(web111a.com.tw)+root(網站根目錄)/新增資料夾(web111a)/80改為6080/ -->