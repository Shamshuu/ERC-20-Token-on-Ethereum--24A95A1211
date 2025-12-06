# ERC-20-Token-on-Ethereum--24A95A1211

## Overview
MyToken is a simple, beginner-friendly ERC-20 token built on the Ethereum blockchain.  
It demonstrates essential token mechanics such as transfers, allowances, and event emission, making it an ideal introduction to smart contract development.

## Token Details
- **Name:** MyToken  
- **Symbol:** MTK  
- **Decimals:** 18  
- **Total Supply:** 1,000,000 MTK (minted to the deployer)

## Features
- Fully ERC-20 compatible  
- Transfer tokens between addresses  
- Approve spenders using the allowance mechanism  
- transferFrom for third-party token transfers  
- Transfer and Approval events for transparency  
- Balance and allowance tracking  
- Optional helper functions (getTotalSupply, getTokenInfo)

## How to Deploy
1. Open RemixIDE at https://remix.ethereum.org  
2. Create `MyToken.sol`  
3. Paste your contract code  
4. Compile with Solidity 0.8.x  
5. Deploy with total supply (in smallest units)

## How to Use

### Check Balance
```
balanceOf(address account) → uint256
```

### Transfer Tokens
```
transfer(address to, uint256 amount) → bool
```

### Approve Spending by Another Address
```
approve(address spender, uint256 amount) → bool
```

### Transfer Tokens on Behalf of an Owner
```
transferFrom(address from, address to, uint256 amount) → bool
```

## Event Logs

### Transfer
```
event Transfer(address indexed from, address indexed to, uint256 value);
```

### Approval
```
event Approval(address indexed owner, address indexed spender, uint256 value);
```

## Testing Steps
- Deploy using JavaScript VM  
- Test transfer, approve, transferFrom  
- Test edge cases (zero address, insufficient balance/allowance)

## License
MIT License
