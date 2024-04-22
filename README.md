# Voting system

This is a voting system using the blockchain concept

## Dependencies

- Node
- Truffle ```npm install -g truffle```
- [Ganache](https://archive.trufflesuite.com/ganache/)
- [Metamask](https://metamask.io/)

You will need to connect your Ganache server to localhost, you can follow this [tutorial](https://docs.cranq.io/web-3/setting-up-ganache-with-metamask)
You can import ETH from your ganache account

## How to use

### Run the project

1. ```truffle migrate``` or ```truffle migrate --reset``` if you want to chaneg your smart contracts
2. ```npm run dev``` the application will be accessible on [http://localhost:3000](http://localhost:3000)
3. ```truffle test``` to run the unit test

### Change the candidates

You can add/update the candidate list in [Election.sol](./contracts/Election.sol) in the constructor

```sol
constructor () public {
    addCandidate("Candidate 1");
    addCandidate("Candidate 2");
}
```