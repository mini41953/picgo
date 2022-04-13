# XAMPP 的建置

## 環境條件
- php 7.4.24
- mysql
- xampp-windows

## 建置虛擬主機
1.條件:
  - 主機名稱: web111a
  - 網址: com.tw
  - 網站根目錄: C:\xampp\htdocs\web111a

2.設置步驟:

  2.1修改虛擬主機設定檔:`C:\xampp\apache\conf\extra\httpd-vhosts.conf` 如下:

<!-- httpd-vhosts.conf 開啟/最下方 複製 註解拿掉/修改seveer name(web111a.com.tw)+root(網站根目錄)/新增資料夾(web111a)/80改為6080/ -->

`
<VirtualHost *:6080>
    ##ServerAdmin webmaster@dummy-host2.example.com
    DocumentRoot "C:/xampp/htdocs/web111a"
    ServerName web111a.com.tw
    ##ErrorLog "logs/dummy-host2.example.com-error.log"
    ##CustomLog "logs/dummy-host2.example.com-access.log" common
</VirtualHost>
`

  2.2設置主機對應IP，添加訊息於`C:\Windows\System32\drivers\etc`

  127.0.0.1 web111a.com.tw

  >使用指令`ipconfig`來查詢自己電腦上的`Ip`

  
<!-- DNS 外網 domain nic -->
<!-- www.hinet.net -->
<!-- ping web111a.com.tw -->
<!-- 系統管理員執行nopad/(C:\Windows\System32\drivers\etc)/ipconfig -->
<!-- doc/ping 127.0.0.1 || ping localhost || ping web111a.com.tw -->
<!-- mysqld -version -->


3.測試
虛擬主機設定檔修改完成後，重新啟動伺服器，打開瀏覽器輸入網址：`http://web111a.com.tw:6088`

`產出PDF檔
1.F1
2.搜尋 "ma


