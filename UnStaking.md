![배너 전환(0 7X3m)](https://github.com/user-attachments/assets/eda143b6-e44e-436c-bd07-057f6a2a4dc5)


## Origin 한국 유저를 위해 작성된 메뉴얼입니다.
###### DApp 에 접근 불가상황에 아래의 순서대로 따라하시면 언스테이킹이 가능합니다. Dapp 에서 언스테이킹 권한 설정이 된 경우에 정상 작동합니다.
#
###### TokenPocket, MetaMask 등 지갑 앱 메뉴 중 DApps 항목의 브라우저 기능을 활용하시는걸 추천합니다.
#
### 1. 언스테이킹 실행을 위해 아래 코드창 오른쪽 버튼 <img width="38" alt="Copy" src="https://github.com/user-attachments/assets/3e2d6b1b-e0fd-4c5f-a8b7-644a13e38e67"/> 모양과 같은 아이콘 버튼 클릭하여 복사한 후 아래로 스크롤을 내려서 2번 항목으로.
#
```
[
    {
      "inputs": [
        { "internalType": "address", "name": "_OHM", "type": "address" },
        { "internalType": "address", "name": "_sOHM", "type": "address" },
        { "internalType": "uint256", "name": "_epochLength", "type": "uint256" },
        { "internalType": "uint256", "name": "_firstEpochNumber", "type": "uint256" },
        { "internalType": "uint256", "name": "_firstEpochBlock", "type": "uint256" }
      ],
      "stateMutability": "nonpayable",
      "type": "constructor"
    },
    {
      "anonymous": false,
      "inputs": [
        { "indexed": true, "internalType": "address", "name": "previousOwner", "type": "address" },
        { "indexed": true, "internalType": "address", "name": "newOwner", "type": "address" }
      ],
      "name": "OwnershipPulled",
      "type": "event"
    },
    {
      "anonymous": false,
      "inputs": [
        { "indexed": true, "internalType": "address", "name": "previousOwner", "type": "address" },
        { "indexed": true, "internalType": "address", "name": "newOwner", "type": "address" }
      ],
      "name": "OwnershipPushed",
      "type": "event"
    },
    {
      "inputs": [],
      "name": "XPH",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [{ "internalType": "address", "name": "_recipient", "type": "address" }],
      "name": "claim",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "contractBalance",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "distributor",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "epoch",
      "outputs": [
        { "internalType": "uint256", "name": "length", "type": "uint256" },
        { "internalType": "uint256", "name": "number", "type": "uint256" },
        { "internalType": "uint256", "name": "endBlock", "type": "uint256" },
        { "internalType": "uint256", "name": "distribute", "type": "uint256" }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    { "inputs": [], "name": "forfeit", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [{ "internalType": "uint256", "name": "_amount", "type": "uint256" }],
      "name": "giveLockBonus",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "index",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "locker",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "manager",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    { "inputs": [], "name": "pullManagement", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [{ "internalType": "address", "name": "newOwner_", "type": "address" }],
      "name": "pushManagement",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    { "inputs": [], "name": "rebase", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    { "inputs": [], "name": "renounceManagement", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [{ "internalType": "uint256", "name": "_amount", "type": "uint256" }],
      "name": "returnLockBonus",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "sXPH",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        { "internalType": "enum OlympusStaking.CONTRACTS", "name": "_contract", "type": "uint8" },
        { "internalType": "address", "name": "_address", "type": "address" }
      ],
      "name": "setContract",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [{ "internalType": "uint256", "name": "_warmupPeriod", "type": "uint256" }],
      "name": "setWarmup",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [
        { "internalType": "uint256", "name": "_amount", "type": "uint256" },
        { "internalType": "address", "name": "_recipient", "type": "address" }
      ],
      "name": "stake",
      "outputs": [{ "internalType": "bool", "name": "", "type": "bool" }],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    { "inputs": [], "name": "toggleDepositLock", "outputs": [], "stateMutability": "nonpayable", "type": "function" },
    {
      "inputs": [],
      "name": "totalBonus",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [
        { "internalType": "uint256", "name": "_amount", "type": "uint256" },
        { "internalType": "bool", "name": "_trigger", "type": "bool" }
      ],
      "name": "unstake",
      "outputs": [],
      "stateMutability": "nonpayable",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "warmupContract",
      "outputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [{ "internalType": "address", "name": "", "type": "address" }],
      "name": "warmupInfo",
      "outputs": [
        { "internalType": "uint256", "name": "deposit", "type": "uint256" },
        { "internalType": "uint256", "name": "gons", "type": "uint256" },
        { "internalType": "uint256", "name": "expiry", "type": "uint256" },
        { "internalType": "bool", "name": "lock", "type": "bool" }
      ],
      "stateMutability": "view",
      "type": "function"
    },
    {
      "inputs": [],
      "name": "warmupPeriod",
      "outputs": [{ "internalType": "uint256", "name": "", "type": "uint256" }],
      "stateMutability": "view",
      "type": "function"
    }
  ]
```
#
### 2. 스마트 컨트랙 도구 실행 => [클릭](https://ethereum-smart-contract-interaction-tool.vercel.app).
#
### 3. 스마트 컨트랙 도구 창과 사용자 본인의 디지털 웰렛 연결.
![smart-contract_002](https://github.com/user-attachments/assets/1f35958e-717b-4d12-aeda-96f0e06e7021)
#
### 4. 스마트 컨트랙 도구 창의 "Paste ABI JSON here" 에 붙여넣기
![smart-contract_003](https://github.com/user-attachments/assets/f091376b-7438-49a4-96c3-bb1a79696b5b)
#
### 5. 스테이킹 주소 복사 (아래 코드창 오른쪽 버튼 <img width="38" alt="Copy" src="https://github.com/user-attachments/assets/3e2d6b1b-e0fd-4c5f-a8b7-644a13e38e67"/> 모양과 같은 아이콘 버튼 클릭하여 복사!!!)
```
0x1964Ca90474b11FFD08af387b110ba6C96251Bfc
```
#
### 6. 스마트 컨트랙 도구 창의 "Contract Address" 에 붙여넣기.
![smart-contract_005](https://github.com/user-attachments/assets/787f9549-f2e2-4132-ba54-558b52511d0d)
#
### 7. 화면 하단에 "Write Function: unstake" 메뉴 찾기.
![smart-contract_006-2](https://github.com/user-attachments/assets/f6eaf285-5d2d-46ca-9056-80dea9bc8755)
#
### 8. unstake 수량 입력.
![smart-contract_007](https://github.com/user-attachments/assets/713898b2-c1c2-4a42-a2c5-b7193f9aa3e3)
@ LGNS 수량 입력 예:
| 언스테이킹 하려는 수량      | 0.01 | 0.1     | 1      | 12 | 123     | 1,234      |
|    :----:   |    :----:   |    :----:   |    :----:   |    :----:   |    :----:   |    :----:   |
| _amount 박스에 입력 값      | 10000000       | 100000000   | 1000000000      | 12000000000       | 123000000000   | 1234000000000      |
| 0 이 입력되는 수   | 7        | 8      | 9   | 9        | 9      | 9   |
#
### 9. CALL UNSTAKE 실행.
![smart-contract_008](https://github.com/user-attachments/assets/1938688a-59c7-477d-b797-3a57477d2501)
##
### 10. 토큰 포켓, 메타마스크 등 개인 지갑에 LGNS 토큰으로 해제된 수량 확인.
