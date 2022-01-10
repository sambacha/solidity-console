# Contract Testing Library 


### LibHEVM

```json
{
	"kind": "user",
	"methods": {
		"addr(uint256)": {
			"notice": "Gets address for a given private key, (privateKey) => (address)"
		},
		"deal(address,uint256)": {
			"notice": "Sets an address' balance, (who, newBalance)"
		},
		"etch(address,bytes)": {
			"notice": "Sets an address' code, (who, newCode)"
		},
		"expectRevert(bytes)": {
			"notice": "Expects an error on next call"
		},
		"fee(uint256)": {
			"notice": "Set block.basefee (newBasefee)"
		},
		"ffi(string[])": {
			"notice": "Performs a foreign function call via terminal, (stringInputs) => (result)"
		},
		"load(address,bytes32)": {
			"notice": "Loads a storage slot from an address (who, slot)"
		},
		"prank(address)": {
			"notice": "Sets the *next* call's msg.sender to be the input address"
		},
		"roll(uint256)": {
			"notice": "Set block.height (newHeight)"
		},
		"sign(uint256,bytes32)": {
			"notice": "Signs data, (privateKey, digest) => (r, v, s)"
		},
		"startPrank(address)": {
			"notice": "Sets all subsequent calls' msg.sender to be the input address until `stopPrank` is called"
		},
		"stopPrank()": {
			"notice": "Resets subsequent calls' msg.sender to be `address(this)`"
		},
		"store(address,bytes32,bytes32)": {
			"notice": "Stores a value to an address' storage slot, (who, slot, value)"
		},
		"warp(uint256)": {
			"notice": "Set block.timestamp (newTimestamp)"
		}
	},
	"version": 1
}
