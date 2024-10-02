<h2 align=center> Fhenix Dev Task </h2>

## Join Discord
- First join [Fhenix Discord](https://discord.gg/fhenix-io)
- Visit `#🤖|bot-commands` and write `/quests` and select the popped up `/quests` option and then press `Enter`

![Img-1](https://github.com/user-attachments/assets/30f7abde-4ab0-4d7b-9b53-4101a7028e7e)

- You will see 10 different quests, here I will show how to do only dev tasks (`Quest 4`,`Quest 6`,`Quest 7`)

---

## Network Set Up
- Visit [Chainlist](https://chainlist.org/?testnets=true&search=Fhenix+Helium)
- Click on `Connect wallet` and then add the network in your preferred wallet (Metamask or Rabby or OKX)

---

## Faucet (Bridge)
- Right now you can get tFHE faucet by mining [here](https://get-helium.fhenix.zone/)
- You can also get tFHE by bridging from the below website

1. [Native Bridge](https://bridge.helium.fhenix.zone/) [Sepolia Ethereum -> Fhenix Helium]
2. [Pheasant Bridge](https://testnet.pheasant.network/) [Many other testnet networks supported]

## Quest 4 : Deploy Contract on Fhenix
- Visit [Remix Website](https://remix.ethereum.org)
  
![Img-2](https://github.com/user-attachments/assets/f186a74b-3287-478a-a14b-7ca267aa9f18)

- Give it any name but at the last part u need `.sol` as this is a solidity file [Example : `zun.sol`] and then press `Enter`
- After that you will an interface like this 

![image](https://github.com/user-attachments/assets/b9a9a624-2733-4393-b014-b4e995e01c0c)

- You need copy the below mentioned codes and paste it there

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract FollowPrompt {
    string private greetingMessage;

    constructor() {
        greetingMessage = "Follow @ZunXBT on X!";
    }

    function setGreeting(string memory newGreeting) public {
        greetingMessage = newGreeting;
    }

    function greet() public view returns (string memory) {
        return greetingMessage;
    }
}
```
