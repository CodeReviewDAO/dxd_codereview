### Test LiquidNFT-Factory Flows

* **Main Contract Flow Test:**

```
~/CasperLabs-LiquidNFT/JsClients/LiquidNFT-Factory-Tests-Scripts/mainContractFlowScript$ npm run testMainContractFlow 23 name AwesomeNFT f7e686e9086b54918896bda93b490d878abf9a4c35006f68f8fb6ce8811cdff0 5c89f407dacab04f69b704a81c6786b9e115ea3dcea6499d6a95203bece6c406 4000000000 10000000000 86400000 10 4efb977f33caaddc15ebd244a1245b3e930cc9fc898b98792688ba7ecfad4c04 keys 1000000000000 5000000000 1000000000 1000000000

> LiquidNFT-Factory-JsClient-mainContractFlowScript@0.0.0 testMainContractFlow
> ts-node script/testMainContractFlow.ts

... Mint deploy hash:  ec3240fd1047aaf0aef29698e698f337d03e3c14992a948c59ade1da3ffe7942
... Token minted successfully.
... Approve deploy hash:  6e04f0c69efab36fc695beec46b1b4686942c22c5ab8c3aa56dae58a5a68fc7d
... Token approved successfully
... createLiquidLockerJsClient deploy hash:  e627f3e0e33c3b5f7987fb8a7ea959ed502c7319ed339ec3e1671d29d0ecece0
... createLiquidLockerJsClient function called successfully
... Mint deploy hash:  bee0a2997e5494a5b258e24dda0821d5262e4c2eac6ca6404609014499324109
... Token minted successfully.
... Approve deploy hash:  ecced2aeb21e8e225adec75d4ea15cd6085dfa0cdfa8dbd593f8ccddab5bef48
... Token approved successfully.
... contributeToLockerJsClient deploy hash:  091fc6d92a2e6c909e756258510b44a9aa471121543b50745d367b0a643529bf
... contributeToLocker function called successfully
... enableLocker deploy hash:  908837205e92b3c8e144a3371ed8168b1b43090762dd9e6c02db9a6ecaf58bd6
... enableLocker function called successfully
... paybackToLocker deploy hash:  71e40e6e00fd047fcd8c6373ba81fcc9b9ab6ac210ddc9552b1aff2870f25357
... paybackToLocker function called successfully


------
```

* **TooLate Payment Liquidate Flow Test:**

``` 
~/CasperLabs-LiquidNFT/JsClients/LiquidNFT-Factory-Tests-Scripts/tooLateLiquidateFlowScript$ npm run testTooLatePayBackFlow 32 name AwesomeNFT d10359a72bdf42adbe6067b4e7c1c16ccf199e6329a9aeef32c02d40b36ea0fe 5c89f407dacab04f69b704a81c6786b9e115ea3dcea6499d6a95203bece6c406 4000000000 10000000000 120000 10 4efb977f33caaddc15ebd244a1245b3e930cc9fc898b98792688ba7ecfad4c04 keys 1000000000000 5000000000 1000000000 1000000000

> LiquidNFT-Factory-JsClient-tooLateLiquidateFlowScript@0.0.0 testTooLatePayBackFlow
> ts-node script/testTooLatePayBackFlow.ts

... Mint deploy hash:  7fcc0bc83eaf6402d6c1757dff7131d827d366e8903e0107296cfbcea0cafa57
... Token minted successfully.
... Approve deploy hash:  ccc9689282c9b5e8e0ad6c2c7ab2c22347cc6526d0def06249d967e0b5ac6d9c
... Token approved successfully
... createLiquidLockerJsClient deploy hash:  88c172bb6e47a12b4649cd6daaa78a4117b834c6d8992e1c156cfcc04365cbe6
... createLiquidLockerJsClient function called successfully
... Mint deploy hash:  239edc26b78b6a5b15579f3d21cee4bba8778c1bf3f73bf244478d8d0ee51f57
... Token minted successfully.
... Approve deploy hash:  3a31bfdcef331a58ef86131ef44077e9f90b36c1f3afbedfb913450564c54054
... Token approved successfully.
... contributeToLockerJsClient deploy hash:  e7101ca319b0ddf7d8c4efc2e809e95e0b631a3e5033864f009ea4dffb0e4b5f
... contributeToLocker function called successfully
... enableLocker deploy hash:  7b4fd4cfd331f66ae4eaa7b7985e052f6324a3e7bcb8fa7b0bd3ca6cb76d34bb
... enableLocker function called successfully
... paybackToLocker deploy hash:  23230f6a2591048b0b24e5723ff1137a5a8cf8505a0bf632e99bf1284a7d7123
... paybackToLocker function called successfully
...liquidateLocker deploy hash:  1344d71e88096e76067d44b7ce801686e4edf3c80141b847c95ee704ddd31a28
... liquidateLocker function called successfully
```
