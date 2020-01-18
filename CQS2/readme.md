A very simple example app using Connext.


Clone the app, and install the node packages with...
`npm install`

Then start the app using...
`npm start`

Might have to upgrade eccrypto dependency separately.
```
cd node_modules/eccrypto
npm run install
```

## Docker mode

If the following does work for whatever reason, try running this app in Docker!

The only prerequisite is [installing docker](https://docs.docker.com/docker-for-mac/install/).

```
npm run build
```

This will build the docker image according to recipe outlined in Dockerfile.

```
npm run start-docker
```

This will execute the docker image. It includes the flag `--mount=type=bind,source=`pwd`/src,target=/root/src` which mounts the `src` folder into the docker image. This means we don't need to rebuild the image every single time the source code changes (Ditto for the .env file).

Address:

Address: 
BIP32 Extended Public Key, a.k.a. xPub: xpub6DqrDxhK5JXDugGw3ibKDyeHydGyL6nTWD6Us4XBWFPQRDciaqD41yG2LZMYgn1rLKh75MLT9tacB9siukrcyLwTne7eYYoTwFTpCgWun7d


Example of state:
```
info: [ConnextClient] Found state to restore from node: {
  "multisigAddress": "0x7Faf6D1B07e7E04F2Ea826a2CC01C400a830d85f",
  "proxyFactoryAddress": "0x8eb543b35DE94B0E636402C7cA32947b22853eDF",
  "userNeuteredExtendedKeys": [
    "xpub6DZv6JzHGBAqDnJ8CLgy3cuVLsMYTeK4vRuycDEdYcmTo3cehiDg46iShdwzyWEG11DUbTQKETGVqPhAa9Ns7gbjFE7ajmW9n8fQj6XmSQa",
    "xpub6DtNpvWhpYY4gPYcGBcUhBAorEbkzCxBUdbfS4DHKjnHJGPxe5YQ7KpFSuW3Z9JHS29uMqJ3HNvzZTkVrbRGSfhaySUiNUPddKUV9NePp5m"
  ],
  "proposedAppInstances": [
    [
      "0x47e4bcd488b178c58c417d7726072c274171302f04835f8a9684c45b13b87fde",
      {
        "appDefinition": "0x08572D3Ecd567d354e679A5bceCBB5c1Ac5f1a59",
        "abiEncodings": {
          "actionEncoding": "tuple(bytes32 preImage)",
          "stateEncoding": "tuple(tuple(address to, uint256 amount)[2] coinTransfers, bytes32 linkedHash, uint256 amount, address assetId, bytes32 paymentId, bytes32 preImage)"
        },
        "initialState": {
          "amount": "100000000000000000",
          "assetId": "0x0000000000000000000000000000000000000000",
          "coinTransfers": [
            {
              "amount": "100000000000000000",
              "to": "0x5307B4F67ca8746562A4a9fdEb0714033008Ef4A"
            },
            {
              "amount": "0",
              "to": "0xFA19fd0dF5B1389ff4a1dB87D608BBE7bAfBF092"
            }
          ],
          "linkedHash": "0x8b2820dcebffea19152023529fcae0f81c3377173d659db1153a44654e2e4bad",
          "paymentId": "0x6dabe3ac49b3f7b7ec8e97940810e4ff6be7b583a84ba72df80a3e8db73db9bc",
          "preImage": "0x0000000000000000000000000000000000000000000000000000000000000000"
        },
        "outcomeType": "SINGLE_ASSET_TWO_PARTY_COIN_TRANSFER",
        "initiatorDeposit": "0x016345785d8a0000",
        "responderDeposit": "0x00",
        "timeout": "0x00",
        "identityHash": "0x47e4bcd488b178c58c417d7726072c274171302f04835f8a9684c45b13b87fde",
        "proposedByIdentifier": "xpub6DZv6JzHGBAqDnJ8CLgy3cuVLsMYTeK4vRuycDEdYcmTo3cehiDg46iShdwzyWEG11DUbTQKETGVqPhAa9Ns7gbjFE7ajmW9n8fQj6XmSQa",
        "proposedToIdentifier": "xpub6DtNpvWhpYY4gPYcGBcUhBAorEbkzCxBUdbfS4DHKjnHJGPxe5YQ7KpFSuW3Z9JHS29uMqJ3HNvzZTkVrbRGSfhaySUiNUPddKUV9NePp5m",
        "appSeqNo": 14,
        "initiatorDepositTokenAddress": "0x0000000000000000000000000000000000000000",
        "responderDepositTokenAddress": "0x0000000000000000000000000000000000000000"
      }
    ]
  ],
  "appInstances": [],
  "freeBalanceAppInstance": {
    "participants": [
      "0x5307B4F67ca8746562A4a9fdEb0714033008Ef4A",
      "0xFA19fd0dF5B1389ff4a1dB87D608BBE7bAfBF092"
    ],
    "defaultTimeout": 172800,
    "appInterface": {
      "addr": "0xde8d1288e2c7eC3e0b7279F8395b87A996Cc02f4",
      "stateEncoding": "tuple(address[] tokenAddresses, tuple(address to, uint256 amount)[][] balances, bytes32[] activeApps)"
    },
    "isVirtualApp": false,
    "appSeqNo": 0,
    "latestState": {
      "activeApps": [],
      "tokenAddresses": [
        "0x0000000000000000000000000000000000000000"
      ],
      "balances": [
        [
          {
            "to": "0x5307B4F67ca8746562A4a9fdEb0714033008Ef4A",
            "amount": "0"
          },
          {
            "to": "0xFA19fd0dF5B1389ff4a1dB87D608BBE7bAfBF092",
            "amount": "1100000000000000000"
          }
        ]
      ]
    },
    "latestVersionNumber": 56,
    "latestTimeout": 172800,
    "outcomeType": "MULTI_ASSET_MULTI_PARTY_COIN_TRANSFER",
    "identityHash": "0x742b88dbf98ef99cfe65dca5bebde448ad238042fb35727a9a62355822059407"
  },
  "monotonicNumProposedApps": 17,
  "singleAssetTwoPartyIntermediaryAgreements": []
}
```
