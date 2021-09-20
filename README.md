# Basic Truffle Ropsten Project

Try running some of the following tasks:

1. Set up Truffle
```shell
npm install -g truffle
npm install --save truffle-hdwallet-provider
```

2. Create your contract in ./contracts

3. Deploy your contract

In ./migrations, create a deployment script specifically named 2_deploy_contracts.js

4. Configure Ropsten network and the provider in truffle.js

Make sure to replace mnemonic and API_KEY with your own.
```shell
truffle deploy --network ropsten
```

5. Access your deployed contract
```shell
truffle console --network ropsten
```

```shell
HelloWorld.deployed().then(function(instance){return instance });
```

6. Finally, invoke contract function and say hello!
```shell
HelloWorld.deployed().then(function(instance){return instance.sayHello()});
```
