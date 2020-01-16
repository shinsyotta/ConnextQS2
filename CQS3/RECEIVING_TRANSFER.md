```
Started to receive transfer with incorrect spelling
info: [ConnextListener] Recieved PROPOSE_INSTALL_EVENT
info: [baseAppValidation] Validating app: {
  "abiEncodings": {
    "stateEncoding": "tuple(address recipient, address multisig, uint256 threshold, address tokenAddress)"
  },
  "appDefinition": "0x11D5f8fB334E7dfBb5555945aF988e9971010325",
  "initialState": {
    "multisig": "0x88A549563399f20d4B6902Db3c9E95D61a54D6B5",
    "recipient": "0x5307B4F67ca8746562A4a9fdEb0714033008Ef4A",
    "threshold": "0",
    "tokenAddress": "0x0000000000000000000000000000000000000000"
  },
  "initiatorDeposit": "0",
  "initiatorDepositTokenAddress": "0x0000000000000000000000000000000000000000",
  "outcomeType": "SINGLE_ASSET_TWO_PARTY_COIN_TRANSFER",
  "proposedToIdentifier": "xpub6Ecyqc2YEBEAVTiry1zfY2YrGHDMoCuo1p9Cv2DbQtg6TRsidCovBBUJ8orY4CPTJib6uMAQPaJ33qL2JgMrKbtq1DqeQysiQ4aRLrjfjPT",
  "responderDeposit": "0",
  "responderDepositTokenAddress": "0x0000000000000000000000000000000000000000",
  "timeout": "0"
}
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for propose protocol
info: [ConnextListener] Sending acceptance message to: indra.client.xpub6Ecyqc2YEBEAVTiry1zfY2YrGHDMoCuo1p9Cv2DbQtg6TRsidCovBBUJ8orY4CPTJib6uMAQPaJ33qL2JgMrKbtq1DqeQysiQ4aRLrjfjPT.proposalAccepted.0x88A549563399f20d4B6902Db3c9E95D61a54D6B5
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for install protocol
info: [ConnextListener] Recieved INSTALL_EVENT
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for install protocol
info: [ConnextListener] Recieved UNINSTALL_EVENT
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for uninstall protocol
info: [ConnextListener] Recieved DEPOSIT_CONFIRMED_EVENT
info: [ConnextListener] Recieved PROPOSE_INSTALL_EVENT
info: [baseAppValidation] Validating app: {
  "abiEncodings": {
    "actionEncoding": "tuple(bytes32 preImage)",
    "stateEncoding": "tuple(tuple(address to, uint256 amount)[2] coinTransfers, bytes32 linkedHash, uint256 amount, address assetId, bytes32 paymentId, bytes32 preImage)"
  },
  "appDefinition": "0x08572D3Ecd567d354e679A5bceCBB5c1Ac5f1a59",
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
        "to": "0xC434C9169Ad0049658CC04336Cb74e35B6Bd4448"
      }
    ],
    "linkedHash": "0xe400523253798f3efe816e611daf9c611a0934fa6e63659f3fb6624077f9ac85",
    "paymentId": "0xfa18510be7ccfa8c3a922e8ea77059a9ef23c049c238e4502cd93c5426993640",
    "preImage": "0x0000000000000000000000000000000000000000000000000000000000000000"
  },
  "initiatorDeposit": "100000000000000000",
  "initiatorDepositTokenAddress": "0x0000000000000000000000000000000000000000",
  "meta": {},
  "outcomeType": "SINGLE_ASSET_TWO_PARTY_COIN_TRANSFER",
  "proposedToIdentifier": "xpub6Ecyqc2YEBEAVTiry1zfY2YrGHDMoCuo1p9Cv2DbQtg6TRsidCovBBUJ8orY4CPTJib6uMAQPaJ33qL2JgMrKbtq1DqeQysiQ4aRLrjfjPT",
  "responderDeposit": "0",
  "responderDepositTokenAddress": "0x0000000000000000000000000000000000000000",
  "timeout": "0"
}
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for propose protocol
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for install protocol
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for install protocol
info: [ConnextListener] not sending propose message, not the coinbalance refund app
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for takeAction protocol
info: [ConnextListener] Recieved UPDATE_STATE_EVENT
info: [ConnextListener] Recieved PROTOCOL_MESSAGE_EVENT for uninstall protocol
Finished receiving transfer with incorrect spelling
info: [ConnextClient] Redeemed transfer {
  "appId": "0x7d1059b88f98007ac02dcc0149b535cf5192d7a4b6f51fe4bbd07bd9f731aa77",
  "freeBalance": {
    "0x5307B4F67ca8746562A4a9fdEb0714033008Ef4A": "0",
    "0xC434C9169Ad0049658CC04336Cb74e35B6Bd4448": "100000000000000000"
  },
  "paymentId": "0xfa18510be7ccfa8c3a922e8ea77059a9ef23c049c238e4502cd93c5426993640"
}
info: [ConnextListener] Successfully redeemed transfer with paymentId: 0xfa18510be7ccfa8c3a922e8ea77059a9ef23c049c238e4502cd93c5426993640
```
