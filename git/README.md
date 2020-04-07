# 前言
版本控制系統大概是最基礎的工具，不管你是在前端、後端還是 APP。熟悉 Git 是基本技能。假設你現在是一個人開發 Web 專案，你至少需要熟悉以下流程。

# 推薦學習資源
中文書：[為你自己學Git](https://gitbook.tw/)

# 問題
- Q1: 請說明
    1. 什麼是版本控制系統？
    -「版本控制系統」，就是指會幫你記錄這些所有的檔案狀態變化，例如每個檔案是誰在什麼時候加進來、什麼時候被修改或刪除，並可以隨時切換到過去某個版本的狀態。
    2. Git 版本控制中有哪幾種檔案狀態？
    - 根據檔案在工作目錄（Working Directory）、暫存區（Staging Area）以及儲存庫（Repository）的位置有：
         - 1.未追蹤(Untracked files)：並沒有被Git所追蹤控管的檔案。
         - 2.已更改(Changes not staged for commit)：已提交版本後，卻又再次修改，這些檔案會被丟回工作目錄。
         - 3.等待提交(Changes to be committed)：在工作目錄的檔案執行git add後，會放在暫存區。這些放在暫存區的檔案狀態便是等待提交。
         - 4.已提交(Committed)：在暫存區的檔案執行git commit後，檔案便置於儲存庫，這些放在儲存庫的檔案即是已提交的狀態。
![](https://i.imgur.com/hZoDAPf.png)
- Q2: 上圖 A-J 是 Git 中檔案狀態切換得流程，請查出 A-J 執行的指令。(重點是確保自己真的學到在什麼情況下使用該指令。)
    - A: 將一般目錄變成 git working folder : git init;
    - B: 將 working folder 的異動狀態登錄到 stage: git add; 
    - C: 將 stage 的狀態放到 local repository: git commit;
    - D: 將 local repository 的狀態放到 remote repository: git push;
    - E: 將 remote repository 的狀態取回到 local repository: git fetch / git pull (git fetch + git merge);
    - F: 將 local repository 的狀態退回到 stage 階段（是 C 的逆向）: git reset --soft;
    - G: 將 stage 的狀態退回到 working folder 階段（是 B 的逆向）: git rm --cached / git reset HEAD;
    - H: 將 local repository 的狀態一口氣退回到 working folder 階段（是 B+C 的逆向）: git reset --mixed;
    - I: 從 remote repository 取回建立成新的 working folder: git clone;
    - J: 將 git working folder 變回一般目錄: rm -rf .git;

- Q3. 做這個題目，你事前評估做了什麼、利用了哪些資源、排程為何、事後怎麼驗收、得到什麼經驗？
   - 事前評估做了什麼：評估自己對這個主題的熟悉度（有學過但需要複習，選擇影片與為你自己學Git先複習再做題）以及預計何時完成（1-2天)。
   - 利用了哪些資源：為你自己學Git以及影片。
   - 排程為何：看完資料後寫題，如果有不確定時，再回去看一遍（整個流程要在禮拜二完成）。
   - 事後怎麼驗收：創一個小檔案練習git的指令，看檔案的狀態是否吻合Q2的要求（git status）。
   - 得到什麼經驗：git是一個入門容易，但隨著專案複雜度上升而需要更加精熟的技巧，只是自己的指令練習，可能無法模擬到真實的多人協作時會遇見的更多程式碼衝突等狀況。
