# tron-api-code-trc20-trx-trc10


Tron-api-Tron interface source code-PHP version-ThinkPHP5 version, if you want to get this source code, in addition to Alipay and QQ, you can also transfer me USDT (150U) through your tron wallet（myaddress：TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny）, and then you can through Telegram (https://t. me/laowu2021) or email (cwwx1818@gmail.com) to contact me to get the source code, as long as the deployment is successful, you can call all the interfaces through the api.

Interface document address: [https://www.showdoc.com.cn/1950021936889677/8867826777420288](https://www.showdoc.com.cn/1950021936889677/8867826777420288)

## Development environment requirements Important reminders:
>
>### 1.php7.3 or 7.4
> ### 2. Install the gmp extension, otherwise the transfer will be unsuccessful
> ### 3. Configure the project pseudo-static
> ### 4. The running directory is public
> ### 5. The contract address does not need to be moved, remember not to change it
> ### 6. ThinkPHP5 basic running requirements, this does not need to be said more
------------

To get the source code, QQ: 1262135552 , wx: bishengshu The reason for adding a friend is specified. Before adding a friend, see the interface document address below


# Tron-api-Tron interface source code-PHP version-ThinkPHP5 version
## The interface document editing time is May 19, 2022 15:50:54
### If you have any questions, you can contact me QQ: 1262135552
### The source code will be updated all the time. The complete source code of the current version of the interface needs to be charged, and the cost is 800 RMB. The package assists in the deployment (the source code is not encrypted)

------------


<!-- ### USDT（150~USDT）



![image](https://user-images.githubusercontent.com/104345258/170924883-33e0abea-ce2e-4ece-88cc-f9b4cdb179c2.png)

 -->
### USDT (150~USDT), Weixinpay(800￥), Alipay (800￥)
##### address：TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny
![image](https://user-images.githubusercontent.com/104345258/169248711-26494e2b-082d-472d-ada9-f0fe2eaa23dd.png)




------------
## TRC20
------------
##### A brief description

- Generate address interface

##### Request URL
- `http://xx.com/api/trc20/generateAddress`
  
##### request method
- GET


##### Return to example

````
{
    "code": 1,
    "data": {
        "privateKey": "41369219ae69fc11ecb589cdd5fdd9a0248918402bdf4d6fe0a7fb6ca752b38b",
        "address": "THJWy3Ej8gv52nmVfWfHZdyRuWX7Qfi3W6",
        "hexAddress": "41506fc7c4241599326c272d26fd08a47f3957d98b"
    }
}
````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|privateKey |string |private key |
|address |string |Wallet address |


------------

##### A brief description

- Get USDT balance interface

##### Request URL
- `http://xx.com/api/trc20/getAddressBalance?address=TGDsEr2cSRC98Zo9WnwNDik2Y5rdboPRvd`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|address |Yes |string |Wallet address to query |

##### Return to example

````
{
    "code": 1,
    "data": "0.00543"
}
````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|data |float |Wallet USDT balance |



------------


    
##### A brief description

- Query order details interface

##### Request URL
- `http://xx.com/api/trc20/transData?txID=40ad467bc5d727164988312e992ea3d7402743d82c4b26244f92ba4194302ce2`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|txID |yes |string |Hash value of the order, the return parameter contains txID |

##### Return to example

````
{
    "code": 1,
    "data": {
        "signature": [],
        "txID": "40ad467bc5d727164988312e992ea3d7402743d82c4b26244f92ba4194302ce2",
        "raw_data": {
            "contract": [
                {
                    "parameter": {
                        "value": {
                            "data": "a9059cbb000000000000000000000416e180a47c9ba3103031151477e35037f7e907eee000000000000000000000000000000000000000000000020000000000020000
                            "owner_address": "4144967f55976c06c4fb55b2e310843c25105ba78d",
                            "contract_address": "41a614f803b6fd780986a42c78ec9c7f77e6ded13c"
                        },
                        "type_url": "type.googleapis.com/protocol.TriggerSmartContract"
                    },
                    "type": "TriggerSmartContract"
                }
            ],
            "ref_block_bytes": "e7d2",
            "ref_block_hash": "82d305046c27b615",
            "expiration": 1648890405000,
            "fee_limit": 100000000,
            "timestamp": 1648890347395
        },
        "contractRet": "SUCCESS"
    }
}
````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|contractRet |string |SUCCESS is success |


------------

    
##### A brief description

- Private key acquisition address interface

##### Request URL
- `http://xx.com/api/trc20/getAddress?privateKey=41369219ae69fc11ecb589cdd5fdd9a0248918402bdf4d6fe0a7fb6ca752b38b`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|privateKey | is |string |private key |

##### Return to example

````
{
    "code": 1,
    "data": {
        "privateKey": "41369219ae69fc11ecb589cdd5fdd9a0248918402bdf4d6fe0a7fb6ca752b38b",
        "address": "THJWy3Ej8gv52nmVfWfHZdyRuWX7Qfi3W6",
        "hexAddress": "41506fc7c4241599326c272d26fd08a47f3957d98b"
    }
}
````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|privateKey |string |Private key address |
|address |string |Wallet address |

--------


    
##### A brief description

- Query the latest block interface

##### Request URL
- `http://xx.com/api/trc20/blockNumber`
  
##### request method
- GET


##### Return to example

````
{
    "code": 1,
    "data": {
        "blockID": "00000000026e6ba7476840363ac0b69de13c3435a883f1492fbe8402424b4868",
        "block_header": {
            "raw_data": {
                "number": 40790951,
                "txTrieRoot": "943b13c18efffc78350606cc341c22f47474f0b5d73b9f43fc051c1b68272820",
                "witness_address": "41c189fa6fc9ed7a3580c3fe291915d5c6a6259be7",
                "parentHash": "00000000026e6ba67909ba661809879ca15c951ef2b80f8cbb8bec5c3bc9db69",
                "version": 23,
                "timestamp": 1652926404000
            },
            "witness_signature": "412e46286ae28d0346f2813b7706a9cbd672e9e40500bc90e196a6315769ec3367ae4bcecad0a32ee17d6dc2aec91dea94f3b9b07bdc38498d106390caf34200"
        },
        "transactions": [
            {
                "ret": [
                    {
                        "contractRet": "SUCCESS"}
                ],
                "signature": [
                    "820cdc956f7d53a18bbeeff0f0eec3c9c933de3d7a75f7e4e795c9393d2d1a9b6a6f47c5ae2994a493ad5d5451fb29617b14c45f5e9178c5f44e99b81804403c01"
                ],
                "txID": "9b3b0004e5a575b3c7a6989d403098a407a5a89b94ea137828eb84a0a32e7180",
                "raw_data": {
                    "data": "436f6e67726174756c6174696f6e73206f6e2067657474696e6720323030e2808b305553e2808b44542c2072656465656d206174202867e2808b6f55e2808b5344e2808b2e56e2808b49502920e88eb7e5be97323030305553e2808b4454efbc8ce588b020676fe2808b7573e2808b642ee2808b76e2808b697020e58591e68da2",
                    "contract": [
                        {
                            "parameter": {
                                "value": {
                                    "amount": 10000000,
                                    "asset_name": "31303034303839",
                                    "owner_address": "41f3e9d30c5db93119cd0ce7a2b9b4ae466173593c",
                                    "to_address": "4145da64cfabd76ff1ad1bfdabf747017b1780bef2"
                                },
                                "type_url": "type.googleapis.com/protocol.TransferAssetContract"
                            },
                            "type": "TransferAssetContract"
                        }
                    ],
                    "ref_block_bytes": "6b93",
                    "ref_block_hash": "fbf1c0822cfcb921",
                    "expiration": 1652926458000,
                    "timestamp": 1652926400907
                },
                "raw_data_hex": "0a026b932208fbf1c0822cfcb9214090d1e0d08d30528101436f6e67726174756c6174696f6e73206f6e2067657474696e6720323030e2808b305553e2808b44542c2072656465656d206174202867e2808b6f55e2808b5344e2808b2e56e2808b49502920e88eb7e5be97323030305553e2808b4454efbc8ce588b020676fe2808b7573e2808b642ee2808b76e2808b697020e58591e68da25a76080212720a32747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e736665724173736574436f6e7472616374123c0a0731303034303839121541f3e9d30c5db93119cd0ce7a2b9b4ae466173593c1a154145da64cfabd76ff1ad1bfdabf747017b1780bef22080ade204708b93ddd08d30"
            }
        ]
    }
}
````
------------

    
##### A brief description

- Query information interface based on blockchain

##### Request URL
- `http://xx.com/api/trc20/blockByNumber?blockID=40743210`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|blockID|Yes |string |BlockID|

##### Return to example

````
{
    "code": 0,
    "msg": "Block not found",
    "data": null,
    "time": 1652926944
}

{
    "code": 1,
    "data": {
        "blockID": "00000000026db12a4392d5f16217affdd5a447a926305a73acd6e4a5cab45b99",
        "block_header": {
            "raw_data": {
                "number": 40743210,
                "txTrieRoot": "790daa73392ad464916dd6f667a6c2369fb341594bff959282be54fbb581b159",
                "witness_address": "4162398d516b555ac64af24416e05c199c01823048",
                "parentHash": "00000000026db1299c08b23996c973834d0b7c6411f0ff6db4243f729b980163",
                "version": 23,
                "timestamp": 1652783076000
            },
            "witness_signature": "6433a64492564e348b2897f5f2d343d046632afba34c030a7e834af4204ad2296188be8b63abf8f7a4d631c885b77e3b7550347833aa83c2f6aaadef4006
        },
        "transactions": [
            {
                "ret": [
                    {
                        "contractRet": "SUCCESS"
                    }
                ],
                "signature": [
                    "3aa5266318c5372bf2fa326134e800f9d714151de01ad07d9c5f2e6d2b71a10f719f4f8284ff3df528e5ded3b1e5c37f5a8ca9b5235e60df300d8448f4cd912b01"
                ],
                "txID": "024872e9db479490be559b62b9cdea0d91de5a176a71ce27e6737d66a5b9b04d",
                "raw_data": {
                    "contract": [
                        {
                            "parameter": {
                                "value": {
                                    "owner_address": "410fe47f49fd91f0edb7fa2b94a3c45d9c2231709c",
                                    "account_address": "416a37c8d377d060c5aeb8677fd95baf0fbd15703b"
                                },
                                "type_url": "type.googleapis.com/protocol.AccountCreateContract"
                            },
                            "type": "AccountCreateContract"
                        }
                    ],
                    "ref_block_bytes": "b116",
                    "ref_block_hash": "a222608fc0c552c6",
                    "expiration": 1652786730000,
                    "timestamp": 1652783072637
                },
                "raw_data_hex": "0a02b1162208a222608fc0c552c64090a8908e8d305a6612640a32747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e4163636f756e74437265617465436f6e7472616374122e0a15410fe47f49fd91f0edb7fa2b94a3c45d9c2231709c1215416a37c8d377d060c5aeb8677fd95baf0fbd15703b70fd8ab18c8d30"
            }
        ]
    }
}
````
------------

    
##### A brief description

- Transaction transfer (offline signature) interface

##### Request URL
- `http://xx.com/api/trc20/transfer?key=41369219ae69fc11ecb589cdd5fdd9a0248918402bdf4d6fe0a7fb6ca752b38b&toaddress=TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny&amount=10`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|key |Yes |string |Transfer wallet private key |
|toaddress |Yes |string | Private key of the receiving wallet |
|amount |No |string | Transfer U amount |

##### Return to example

````
{
    "code": 0,
    "msg": "Transfer Fail",
    "data": null,
    "time": 1652927917
}


{
    "code": 1,
    "data": {
        "signature": [],
        "txID": "ffea9302e47a7fc5511aee58f507a1bf7477f91f491ae66e39ec5505ba54dfe4",
        "raw_data": {
            "contract": [
                {
                    "parameter": {
                        "value": {
                            "data": "a9059cbb00000000000000000000041f5fbe5e8725957174014dca1dc4fed54e970a2f800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000
                            "owner_address": "41f5fbe5e8725957174014dca1dc4fed54e970a2f8",
                            "contract_address": "41a614f803b6fd780986a42c78ec9c7f77e6ded13c"
                        },
                        "type_url": "type.googleapis.com/protocol.TriggerSmartContract"
                    },
                    "type": "TriggerSmartContract"
                }
            ],
            "ref_block_bytes": "6ddf",
            "ref_block_hash": "bfead22de965d544",
            "expiration": 1652928222000,
            "fee_limit": 100000000,
            "timestamp": 1652928165332
        },
        "contractRet": "PACKING"
    }
}


````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|txID |string |The transaction hash is used to query the transaction status of the order asynchronously. Because some transactions may not be received in time, it is necessary to confirm the transaction result asynchronously |
|contractRet |string |This parameter is only successful when it is SUCCESS |




------------

    
##### Brief description (this interface is the official interface)

- Query the latest transaction (USDT) interface

##### Request URL
- `https://api.trongrid.io/v1/accounts/TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny/transactions/trc20?limit=100&contract_address=TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|accounts |Yes |string |The address of the query transaction |

##### Return to example

````
{
    "data": [
        {
            "transaction_id": "d52cd9079cf82595dd507640b7b09e34d2dbb63a56b555355f5ef8984f1eb668",
            "token_info": {
                "symbol": "USDT",
                "address": "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t",
                "decimals": 6,
                "name": "Tether USD"
            },
            "block_timestamp": 1651903617000,
            "from": "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny",
            "to": "TTRmEA73gpoxK2KRmhL7GtcYLh88VefYss",
            "type": "Transfer",
            "value": "15500000"
        },
        {
            "transaction_id": "d2475ca51173ddcacc8f1ebd17f25ffd3f22c9c1b6761c3570010ef9586e9499",
            "token_info": {
                "symbol": "USDT",
                "address": "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t",
                "decimals": 6,
                "name": "Tether USD"
            },
            "block_timestamp": 1651903413000,
            "from": "TTRmEA73gpoxK2KRmhL7GtcYLh88VefYss",
            "to": "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny",
            "type": "Transfer",
            "value": "15500000"
        },
        {
            "transaction_id": "a30518a56c998e8ef33d113c2ef2e9a929faa6eebbcda1d5c432eac2ade41715",
            "token_info": {
                "symbol": "USDT",
                "address": "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t",
                "decimals": 6,
                "name": "Tether USD"
            },
            "block_timestamp": 1651079526000,
            "from": "TDomMB8P1wxbFHdmKhzmX4wpg2o4hn16FV",
            "to": "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny",
            "type": "Transfer",
            "value": "343712"
        }
    ],
    "success": true,
    "meta": {
        "at": 1652928398011,
        "page_size": 3
    }
}
````



------------


    
##### A brief description

- Query all transaction records interface (official, with QPS limit, currently known is 15 QPS)

##### Request URL
- `https://apiasia.tronscan.io:5566/api/transaction?sort=-timestamp&count=true&limit=20&start=0&address=TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny`
  
##### request method
- POST

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|address |Yes |string |Wallet address to query |
|limit |Yes |string | Number of word queries |
|start |No |string | Start bar position |
|sort |No |string | Sort by |

##### Return to example

````
{
    "total": 26,
    "rangeTotal": 26,
    "data": [
   {

    "total": 26,

    "rangeTotal": 26,

    "data": \[

        {

            "block": 40791539,

            "hash": "ffea9302e47a7fc5511aee58f507a1bf7477f91f491ae66e39ec5505ba54dfe4",

            "timestamp": 1652928168000,

            "ownerAddress": "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny",

            "toAddressList": \[

                "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t"

            \],

            "toAddress": "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t",

            "contractType":31,

            "confirmed": true,

            "revert": false,

            "contractData": {

                "data": "a9059cbb00000000000000000000041f5fbe5e8725957174014dca1dc4fed54e970a2f800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000

                "owner\_address": "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny",

                "contract\_address": "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t"

            },

            "SmartCalls": "",

            "Events": "",

            "id": "",

            "data": "",

            "fee": "",

            "contractRet": "REVERT",

            "result": "FAIL",

            "amount": "0",

            "cost": {

                "net\_fee": 0,

                "energy\_usage": 0,

                "fee": 554120,

                "energy\_fee": 554120,

                "energy\_usage\_total": 1979,

                "origin\_energy\_usage": 0,

                "net\_usage": 345

            },

            "tokenInfo": {

                "tokenId": "\_",

                "tokenAbbr": "trx",

                "tokenName": "trx",

                "tokenDecimal": 6,

                "tokenCanShow": 1,

                "tokenType": "trc10",

                "tokenLogo": "https://coin.top/production/logo/trx.png",

                "tokenLevel": "2",

                "vip": true

            },

            "tokenType": "trc10",

            "trigger\_info": {

                "method": "transfer(address \_to,uint256 \_value)",

                "data": "a9059cbb00000000000000000000041f5fbe5e8725957174014dca1dc4fed54e970a2f800000000000000000000000000000000000000000000000000000000000000000000000000000000000000000

                "parameter": {

                    "\_value": "10000000",

                    "\_to": "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny"

                },

                "methodName": "transfer",

                "contract\_address": "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t",

                "call\_value": 0

            }

        }

    \],

    "wholeChainTxCount": 3216646144,

    "contractMap": {

        "TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny": false,

        "TGDsEr2cSRC98Zo9WnwNDik2Y5rdboPRvd": false,

        "TDQpQzXntqM1d5dirPqfUe9rE6BYgqvEok": false,

        "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t": true,

        "TVLNeBgwfB9DvraN92mmWwNJsuV8Fgte4B": false,

        "TNCmcTdyrYKMtmE1KU2itzeCX76jGm5Not": false

    },

    "contractInfo": {

        "TR7NHqjeKQxGTCi8q8ZY4pL8otSzgjLj6t": {

            "tag1": "USDT Token",

            "tag1Url": "https://tron.network/usdt",

            "name": "TetherToken",

            "vip": true

        }

    }

}
````






------------
## TRX

------------

##### A brief description

- Query TRX balance interface

##### Request URL
- `http://xx.com/api/trx/getBalance?address=TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny`
  
##### request method
- POST

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|address |Yes |string |Wallet address to query |


##### Return to example

````
{
    "code": 1,
    "data": 8.2192,
    "msg": "The query succeeded",
    "time": 1652929924
}
````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|data |float |trx balance |





------------

    
##### A brief description

- Query TRX transaction details interface

##### Request URL
- `http://xx.com/api/trx/getTransaction?txID=3189f91d061beddf1f1e3b829768ea2a08cf94c644255f696105587c9fc252b9`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|txID |yes |string |Hash returned by the transfer transaction |

##### Return to example

````
{
    "code": 1,
    "data": {
        "ret": [
            {
                "contractRet": "SUCCESS"
            }
        ],
        "signature": [
            "c7ead724b1d1cad63ed11f2fc86c62e9c1740022fe332ca7fc716819a13f9a377a64ef7c15629b17622dde77f22a35aa5ee22a669f37cc5e4b985eacfcc38b3d00"
        ],
        "txID": "3189f91d061beddf1f1e3b829768ea2a08cf94c644255f696105587c9fc252b9",
        "raw_data": {
            "contract": [
                {
                    "parameter": {
                        "value": {
                            "amount": 1100000,
                            "owner_address": "41f5fbe5e8725957174014dca1dc4fed54e970a2f8",
                            "to_address": "41d46b2c182e2248b98429a384b7cd35616b7e4346"
                        },
                        "type_url": "type.googleapis.com/protocol.TransferContract"
                    },
                    "type": "TransferContract"
                }
            ],
            "ref_block_bytes": "1723",
            "ref_block_hash": "f87ff939116fc43e",
            "expiration": 1652664645000,
            "timestamp": 1652664587529
        },
        "raw_data_hex": "0a0217232208f87ff939116fc43e4088ebf4d38c305a67080112630a2d747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e73666572436f6e747261637412320a1541f5fbe5e8725957174014dca1dc4fed54e970a2f8121541d46b2c182e2248b98429a384b7cd35616b7e434618e091437089aaf1d38c30"
    },
    "msg": "The query succeeded",
    "time": 1652665591
}
````





------------

    
##### A brief description

- TRX transfer interface

##### Request URL
- `http://xx.com/api/trx/send?to=TVLNeBgwfB9DvraN92mmWwNJsuV8Fgte4B&key=41369219ae69fc11ecb589cdd5fdd9a0248918402bdf4d6fe0a7fb6ca752b38b&account=0.1 `
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|to |Yes |string |Receive TRX wallet address |
|key |yes |string | wallet private key to transfer out TRX |
|account |float |string | Amount of TRX transferred |

##### Return to example

````
{
    "code": 0,
    "msg": "class org.tron.core.exception.ContractValidateException : Validate TransferContract error, no OwnerAccount.",
    "data": null,
    "time": 1652930705
}



{
    "code": 1,
    "data": {
        "result": true,
        "txid": "41308bccc46c0c35f92540fafa89a7107c70fd6b63c9bb438d3af234fcf01a20",
        "visible": false,
        "txID": "41308bccc46c0c35f92540fafa89a7107c70fd6b63c9bb438d3af234fcf01a20",
        "raw_data": {
            "contract": [
                {
                    "parameter": {
                        "value": {
                            "amount": 2000000,
                            "owner_address": "41f5fbe5e8725957174014dca1dc4fed54e970a2f8",
                            "to_address": "41d46b2c182e2248b98429a384b7cd35616b7e4346"
                        },
                        "type_url": "type.googleapis.com/protocol.TransferContract"
                    },
                    "type": "TransferContract"
                }
            ],
            "ref_block_bytes": "7181",
            "ref_block_hash": "731656b09870ff3a",
            "expiration": 1652931012000,
            "timestamp": 1652930955144
        },
        "raw_data_hex": "0a0271812208731656b09870ff3a40a0cbf6d28d305a67080112630a2d747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e73666572436f6e747261637412320a1541f5fbe5e8725957174014dca1dc4fed54e970a2f8121541d46b2c182e2248b98429a384b7cd35616b7e43461880897a70888ff3d28d30",
        "signature": [
            "c9540c20572374891f3d61d67be6c6a7401ca437b291828991d68e92f7e6b7295bd27e25742ea74ebb5bf41506cf52917d5204f55427399deecc2b432befffc900"
        ]
    },
    "msg": "Operation successful",
    "time": 1652930955
}

````


##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|result |bool |true means the transaction is successful |
|txID |int |Transaction hash, used for auditing |






------------
## TRC10
------------


    
##### A brief description

- TRC10 transfer interface

##### Request URL
- ` http://xx.com/api/trc10/send?amount=1&address=TYPrKF2sevXuE86Xo3Y2mhFnjseiUcybny&key=41369219ae69fc11ecb589cdd5fdd9a0248918402bdf4d6fe0a7fb6ca752b38b&tokenid=1002992`
  
##### request method
- GET

##### Parameters

|Parameter name|Required|Type|Description|
|:---- |:---|:----- |----- |
|amount |Yes |float |Amount|
|address |Yes |string | Payment address |
|key | yes |string | wallet private key |
|tokenid |yes |string | target token identifier, default 1002992 |

##### Return to example

````
{
    "code": 0,
    "msg": "class org.tron.core.exception.ContractValidateException : No owner account!",
    "data": null,
    "time": 1652932448
}


{
    "code": 1,
    "data": {
        "result": true,
        "txid": "f801555a4ccf6128e31fa96b78c0acf5936df2177d36ea2850033f68bcdf639e",
        "visible": false,
        "txID": "f801555a4ccf6128e31fa96b78c0acf5936df2177d36ea2850033f68bcdf639e",
        "raw_data": {
            "contract": [
                {
                    "parameter": {
                        "value": {
                            "amount": 1,
                            "asset_name": "31303032393932",
                            "owner_address": "4144967f55976c06c4fb55b2e310843c25105ba78d",
                            "to_address": "41f5fbe5e8725957174014dca1dc4fed54e970a2f8"
                        },
                        "type_url": "type.googleapis.com/protocol.TransferAssetContract"
                    },
                    "type": "TransferAssetContract"
                }
            ],
            "ref_block_bytes": "72d6",
            "ref_block_hash": "8dfdfca640ecdaff",
            "expiration": 1652932035000,
            "timestamp": 1652931977809
        },
        "raw_data_hex": "0a0272d622088dfdfca640ecdaff40b883b5d38d305a730802126f0a32747970652e676f6f676c65617069732e636f6d2f70726f746f636f6c2e5472616e736665724173736574436f6e747261637412390a073130303239393212154144967f55976c06c4fb55b2e310843c25105ba78d1a1541f5fbe5e8725957174014dca1dc4fed54e970a2f8200170d1c4b1d38d30",
        "signature": [
            "3b7c9e62adf92e32cf5b06331880606eabdd81f56ce1993b3005cab832000925ec5360fb24927dacf40575b6d1eebcaa4b326047fde0093fbb9555a04b90965c00"
        ]
    },
    "msg": "Transfer successful",
    "time": 1652931977
}
````

##### Return parameter description

|parameter name|type|description|
|:----- |:-----|----- |
|txID |string |Transaction Hash |
