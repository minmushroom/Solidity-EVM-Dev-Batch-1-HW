# hardhat mainnet fork

創建一個 hardhat 資料夾並執行以下代碼安裝所需的 package

```
npm install --save-dev hardhat
npm install --save-dev @nomiclabs/hardhat-waffle ethereum-waffle chai @nomiclabs/hardhat-ethers ethers
```

啟動主網分叉

```
npx hardhat node --fork https://eth-mainnet.alchemyapi.io/v2/<my_key>
```
![image](https://user-images.githubusercontent.com/70627447/148559513-0bf9047d-aa5e-452d-8089-894f9bc6d757.png)

連接小狐狸錢包
![image](https://user-images.githubusercontent.com/70627447/148554665-2935417e-2e9c-4438-af82-a21070442bff.png)


# 用 Ganache-cli 跑 local 的 ethereum mainnet fork
```
ganache-cli-d-fhttps://mainnet.infura.io/v3/<my_key> -u
"0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2" -u "0x5C69bEe701ef814a2B6a3EDD4B1652CB9 cc5aA6f"
-p7545 --defaultBalanceEther 5000
```

