﻿# Change Log
## 1.0.4.4
- Modified ServerConnectionData and MoralisClient to support specification of the Parse Auth Handler.

## 1.0.4.3
- Modified MoralisClient constructor and capture all ServerConnectionData passed in.
- Correct ServerConnectionData to fix double server base issue
- Correct MoralisCloudFunctionService, MoralisFileService, and MoralisObjectService to fix double server base issue.

## 1.0.4.2
This release is a combination of Moralis 1.0 and the new Moralis 2.0 and can be used with either. It is also updated to be able to be used with a self-hosted Parse Server or with the current Moralis Server.

This release has the following major updates:
- New ChainNetworkType enum type in Auth API. You will notice that network enum has both evm and solana but only evm is supported at this time by the Auth 2.0 API.
- Updated endpoints for Auth 2.0 to match the new Api endpoint paths which now include network type.
- Passes X-Api-Key header for Auth 2.0 API calls.
- Updated ServerConnectionData to include Parse Server endpoint definitions.
- Modified MoralisClient constructor.
- Modified Web3Api and SolanaApi was hard coded to the Moralis Server backend endpoints. Self hosted Parse Server can have different endpoint names. These are now pulled from the ServerConnectionData.