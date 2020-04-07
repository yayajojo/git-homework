# 前言
相信大家看過很多電影裡面的帥氣駭客們，總是在黑底白字的介面前面輸入指令操控著電腦。 身為一個工程師，我們當然也要立志當帥氣的工程師，既然如此就得好好學學怎麼使用這烏漆抹黑的介面。

# 推薦學習資源
[鳥哥的 Linux 私房菜](https://linux.vbird.org/linux_basic/centos7/)

# 問題

### 名詞解釋

- GUI vs CLI
  - 圖形介面（GUI，Graphical User Interface）
  - 命令列介面（CLI，Command Line Interface）
  - GUI通常使用大量的按鈕、工具欄、對話方塊等圖示的方式來向計算機發送指令。好處是比起使用純文字的命令列，由於使用者可以較直觀使用圖形介面，因此具有易用性，壞處為圖形介面需要更多計算機系統的資源，效能較差。
CLI採用直接輸入命令和引數的文字列方式直接向計算機發送各種指令。由於可以用純文字發送指令，使得其效率較高與精準，但壞處為使用方式較不直觀，使用者需要記憶操作的命令。
- terminal
  - 終端機 (Terminal)：每個虛擬控制台都會提供一個界面，該界面可以提供鍵盤輸入以及螢幕輸出，這個界面就稱為終端機。 使用者在終端機登入帳號與密碼後，即可取得殼程式 (shell) 來進行系統的互動。一般終端機大多指純文字界面，不過就廣義的說法， 圖形界面 (Graphical User Interface, GUI) 也可視為一種終端機。
- shell
  - 殼程式 (Shell)：讓使用者輸入指令串，然後將該指令串丟進系統執行的軟體，就可稱為是殼程式。
    - bash : Linux 使用的預設版本 Bourne Again SHell (簡稱 bash) 。
    - zsh：基於 ksh 發展出來的，功能更強大的 shell（z shell）。

### 請解釋下方 CLI 的指令作用
    
- `cat`
串接檔案成標準輸出後印出在終端機上
- `cd`
移動所進入的資料夾（change directory)    
- `chgrp`
 改變檔案所屬的群組(change group)
- `chown`
改變檔案擁有者(change owner)
- `chmod`
改變檔案權限(change mode)
- `cp`
複製檔案（copy)
- `curl`
透過其所支持的協定（protocols）向服務器下載和上傳檔案的指令
- `grep`
文字搜尋
- `less`
文件瀏覽
- `ls`
列出目錄中的內容
- `man`
查詢linux線上手冊來找尋某個指令用法
- `mkdir`
 創建新資料夾(make directory)   
- `mv`
移動或重新命名檔案（move/rename) 
- `|`
管線命令的界定符號，管線命令接收標準輸入，並且傳出標準輸出
- `pwd`
印出目前工作目錄（print work directory）
- `rm`
刪除檔案(remove)
- `touch`
用來更新已存在檔案的時間戳記或新增空白檔案
- `vim`
開啟vim編輯器來編輯文字檔案
### 請說明以下 Linux file system structure 

- `/`
根目錄，與開機系統有關
- `/bin`
放置一般使用者可以操作的指令
- `/etc`
放置系統檔案
- `/home`
一般使用者帳戶的家目錄
- `/lib`
系統函式庫與核心函式庫
- `/var`
放置一些變數或記錄檔（variable)
- `/sbin`
放置系統管理員可以操作的指令
- `/srv`
放置網站服務啟動後所需的資料（service)
- `/tmp`
暫存檔案（temporary）
- `/usr`
放置系統相關軟體與服務（unix software resource）
