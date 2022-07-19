将数据添加到 IPFS 并获得 CID 后，就可以准备token的元数据并在区块链上“铸造”token。

生成元数据保存到IPFS（json文件）,在生成CID作为external link

要从智能合约或 NFT 元数据中链接到您的内容，应该将 CID转换为 IPFS URI

要生成 IPFS URI，只需在 CID 字符串前加上静态字符串`ipfs://`



```json
{
  "name": "OG:Crystal 812",    //nft名字
  "description": "This one-of-a-kind OG:Crystal reflects both the remarkable combinations of natural crystalline structures as well as its journey through the crypto wallets of the community. There is no other like it. Welcome to the REEF.",
  //ntf所在位置
  "url": "https://ogcrystals.com",
  //只是封面图
  "image": "https://api.ogcrystals.com/api/v1/crystals/images/original/812/1.jpg", 
  "original": "https://api.ogcrystals.com/api/v1/crystals/images/original/812/1.jpg",
  
  // 对应properties
  "attributes": [
  {
  "trait_type": "Generation",
  "value": "1"
  },
  {
  "trait_type": "Crystallization",
  "value": "Done"
  },
  {
  "trait_type": "Blue",
  "value": "I"
  },
  {
  "trait_type": "Coral",
  "value": "I"
  }
  ]
}
```

![image-20211109172629247](/Users/sens/Library/Application Support/typora-user-images/image-20211109172629247.png)



```json
{
"description": "Metasaurs by Dr. DMT is a collection of 9,999 unique Metasaurs living on the Ethereum blockchain, this time, forever...",
"external_url": "https://metasaurs.com",
"name": "Metasaurs #7565",
"image": "https://mtsr.mypinata.cloud/ipfs/QmPZfiB2fMjKZfKfFPELpwNz7W1aqoJGLdLLapy5v1cWgs/7565.png",
"attributes": [
{
"trait_type": "Background",
"value": "Violet"
},
{
"trait_type": "Clothes",
"value": "Bone Tee"
},
{
"trait_type": "Eyes",
"value": "ETH"
},
{
"trait_type": "Skin",
"value": "Silver"
},
{
"trait_type": "Headgear",
"value": "Fez Cap"
},
{
"trait_type": "Back",
"value": "None"
},
{
"trait_type": "Mouth",
"value": "Meat Mouth"
}
]
}
```



Video not

```json
{
"description": "Tiny Thomasina by Flume x Jonathan Zawada",
"background_color": "ffffff",
"external_url": "https://niftygateway.com/#/",
"image": "https://res.cloudinary.com/nifty-gateway/video/upload/v1617723668/Max/FlumexJonathanZ/Tiny_Thomasina_u87foc.png",
"name": "Tiny Thomasina #9/100",
"animation_url": "https://res.cloudinary.com/nifty-gateway/video/upload/v1617723668/Max/FlumexJonathanZ/Tiny_Thomasina_u87foc.mp4"
}
```





如果传了非图片

![image-20211109181449137](/Users/sens/Library/Application Support/typora-user-images/image-20211109181449137.png)



