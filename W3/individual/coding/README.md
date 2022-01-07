# 安裝 hardhat

轉到一個空文件夾然後開始
```
mkdir Mainnet fork
cd Mainnet fork
```
安裝
```
npm install --save-dev hardhat
npm install --save-dev @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers ethers
```
![image](https://user-images.githubusercontent.com/70627447/148530896-e2b5a9a6-3ac9-4129-b08f-9915e090e56e.png)

## 打開 readme 檔 ， 可以嘗試執行看看這幾個指令
![image](https://user-images.githubusercontent.com/70627447/148531488-51672b6a-9993-453c-9bb8-91ecc314b42c.png)

## 查看 account (npx hardhat accounts)

看一下hardhat.config.js文件，會發現任務的定義accounts
![S__2637846](https://user-images.githubusercontent.com/70627447/148531941-b0fffa10-6985-4a20-8326-62cd9ecc0e2a.jpg)

執行 npx hardhat accounts
```
npx hardhat accounts
```

![image](https://user-images.githubusercontent.com/70627447/148532114-f7b97f70-caa9-4602-a5a9-0d42d249af14.png)

## 編譯合約 (npx hardhat compile)
在 contract 目錄中可以找到 Greeter.sol
![image](https://user-images.githubusercontent.com/70627447/148533034-25eba09d-accb-4a0f-8d78-93dd3d9a9480.png)

執行指令以編譯它
```
npx hardhat compile
```

## 測試合約 (npx hardhat test)
test 目錄中可以找到 sample-test.js 檔案
![image](https://user-images.githubusercontent.com/70627447/148533309-f6de83a8-722c-4b9d-9637-64a5fd7cbec1.png)

打指令以測試合約
```
npx hardhat test
```
![image](https://user-images.githubusercontent.com/70627447/148533543-b89b7584-2b38-4e18-86f6-bb3a1afff222.png)

## 部屬合約 (node scripts/sample-script.js)
在 scripts/ 資料夾中可以發現部屬合約的代碼
![image](https://user-images.githubusercontent.com/70627447/148550697-cb3d44b8-8bd3-4054-a60a-2d79c38c4dda.png)
可以在命令提示字元中輸入以下指令啟動代碼
```
npx hardhat run scripts/sample-script.js
```
![image](https://user-images.githubusercontent.com/70627447/148550764-133b7381-9867-4c93-b4ba-b17d9fc5336f.png)
現在我們已成功部屬合約

## 將錢包或 APP 連到 Hardhap 網路
一般情況下，Hardhap 將啟動在 Hardhat Network 中，以便外部的客戶端能夠連結它
輸入以下指令
```
npx hardhat node
```
![image](https://user-images.githubusercontent.com/70627447/148551321-f5f3fafc-3875-452d-a486-ec05a2e9a0b6.png)
這將向 Hardhat Network 公開一個 JSON-RPC 接口。要使用它，請將錢包或應用程序連接到 `http://localhost:8545`
![image](https://user-images.githubusercontent.com/70627447/148553113-60c9ca59-936e-4b2d-a77f-03fa0067dfdb.png)

