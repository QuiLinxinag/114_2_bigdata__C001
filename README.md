1. 強制切換為 SSH 網址
請直接複製並執行這行，這會覆蓋掉原本那個一直討密碼的 HTTPS 設定：

PowerShell
```
git remote set-url origin git@github.com:QuiLinxinag/114_2_bigdata__LXQ_702.git
```
2. 確認網址是否更改成功
輸入以下指令檢查：

PowerShell
```
git remote -v
、、、
預期結果： 你應該會看到兩行都以 git@github.com:... 開頭。如果還是看到 https://，代表沒設定成功。

3. 再次推送
現在連線已經換成 SSH 了，請再推一次：

PowerShell
```
git push -u origin main
、、、
