# Ontology Web3 Domains

Nodejs SDK

Npm: https://www.npmjs.com/package/domainchainjs

Before installing the package you need to check and be sure to install the packages below:

```
npm install web3 
```

Install Package

```
npm install domainchainjs
```

Call 
```
const domainchainjs = require('domainchainjs');
```

Install:

```
const onto = 
{
	"rpcUrl": "https://dappnode1.ont.io:10339",
	"contractAddress": "0x17504d8dd22820e3209d92b838c089647b98d526"		
}
const sdk = domainchainjs.SDK('custom', onto); 

// your domains
const _domain = "hello.ont";
	
// resolve domain to get the address of the owner.
const owner = await sdk.getOwner(_domain);

console.log(owner);

// your address
const _address = "0x5aEa3F3f358347Abf94B554389174F966faeEfbB";

// get a domain default from a user's address, requiring the user to set the default domain name initially.
const domain = await sdk.getDomain(_address);

console.log(domain);
```
Pls update test.js for specific instructions

Thanks!



