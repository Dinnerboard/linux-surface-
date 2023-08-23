# linux-surface-camera 在linux-surface設備上安裝攝像頭驅動
參考：https://github.com/linux-surface/
本教程旨在完成原文的中文本地化翻譯及相關補充
基於Ubuntu系統，其他請自行參考原文檔，無太大差異


1.安裝linux-surface核心
參考：https://github.com/linux-surface/linux-surface/wiki/Installation-and-Setup
注意：在安裝安全啓動密鑰之後，此套件將向終端列印說明。如果您錯過了這些：它會要求您重新啟動。然後，重新啟動時，應彈出一個藍色功能表，詢問您是否要註冊密鑰。使用 / 確認 ok ， 並要求輸入密碼時輸入 surface yes 如果您錯過了功能表或意外選擇了錯誤的選項，您可以卸載（完全），然後重新安裝軟體包並重新啟動以再次觸發功能表。

如果您錯過了該怎麼辦？
1.（刪除錯誤內核）打開終端機，輸入
dpkg --list | grep linux-image
此操作會顯示所有已安裝的內核，找到名字中帶有surface的內核，復制名字
2.輸入
sudo apt-get remove \內核名字
3.（刪除安全啓動密鑰）輸入
sudo apt remove linux-surface-secureboot-mok
4.重新啓動，重置完成，接下來您可以按照原文進行重新安裝


2.安裝攝像頭驅動
參考：https://github.com/linux-surface/linux-surface/wiki/Camera-Support




