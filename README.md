## ð« **Near Election Contract**

## Web ãµã¤ã

ä½ææ¸ã¿ã®ã¢ããªãè¦ããæ¹ã¯[ãã¡ã](https://tonny-near-election-dapp.netlify.app/)ãããè¦§ãã ããã

## **Quick Start**

---

1. [ãã¡ã](https://wallet.testnet.near.org/)ã§æ°ãã wallet ãä½æãã¦ãã ãã

2. ä½æãã Wallet ã® ID ã`YOUR_WALLET_ID`ã«ä»£å¥ãã¦ãä¸ã®ã³ã¼ããã¿ã¼ããã«ã§èµ°ããã¦ãã ããã

```
    export NFT_CONTRACT_ID="YOUR_WALLET_ID"
```

ï¼ä¾ãã° YOUR_CONTRACT_ID ã«ã¯ dev_account.testnet ãªã©ãå¥ããã¨ã«ãªãã¾ã)

3. ä¸ã®ã³ã¼ããã¿ã¼ããã«ã§èµ°ããã¦ã­ã°ã¤ã³ãã¦ãã ãã

```
    near login
```

4. ä¸ã®ã³ã¼ããã¿ã¼ããã«ã§èµ°ããã¦ã³ã³ãã¤ã«ãããã­ã¤ãã³ã³ãã©ã¯ãã®åæåããã¦ãã ãã

```
    near deploy --wasm-file target/wasm32-unknown-unknown/release/near_voting_contract.wasm --accountId $NFT_CONTRACT_ID && near call $NFT_CONTRACT_ID new_default_meta '{"owner_id": "'$NFT_CONTRACT_ID'"}' --accountId $NFT_CONTRACT_ID
```

3. ããã§ã³ã³ãã©ã¯ãã®æºåã¯å®äºã§ããã§ã¯[ãã¡ã](https://github.com/honganji/near-election-dapp-frontend)ããã³ã¼ãã clone ããå¾ãREADME.md ã®éãã«æºåããã¦ã¢ããªãèµ·åããã¾ãããï¼
