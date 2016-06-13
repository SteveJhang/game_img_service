# game_img_service

此組態設定檔是使用Ansible來佈署遊戲映像檔下載服務，並監控伺服器的流量。

分為兩部份：

A. 基礎環境套件安裝  

   1.先用img-service.yml 安裝套件(apache、vsftp、snmp)。    
   
B. 使用者上傳檔案帳號（FTP）  

   1.用useraccount.yml產生新的使用者帳號。  
     
   使用usetaccount.yml 需要輸入username&password。  
     
   2.重啟服務生效設定。  

C. 上傳映像檔到伺服器，和提供玩家下載硬像檔  

   FTP HOST: username.example.com.tw  
   
   上傳一個game.iso到FTP
   
   下載路徑為： http://username.example.com.tw/game.iso
   
