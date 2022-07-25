## Unit 3: Ethereum | Local Development Environments -English Version- 🚀

### Save people array! 

This smart contract will allow you to store and retrieve a person name and favorite number

Please use the methods: 

1) store(string,uint256) : Call this method to store the persona name and favorite number as parameters. For instance: store('Vanessa',150). The smart contract stores an array of people, so you can call this method several times.

2) searchFavoriteNumberPerPerson(string) : Call this method to retrieve the favorite number of a given person by name. For instance: searchFavoriteNumberPerPerson('Vanessa') will return 150.

3) retrieve(uint256) : Call this method to retrieve person data by index. For instance, if the first person you store is 'Vanessa', then calling retrieve(0) will return (name:'Vanessa', favoriteNumber: 150)

### Deployment

This smart contract is ment to be deployed in a ganache network: truffle-config.js looks like following: 

module.exports = {
  compilers: {
    solc: {
      version: "0.8.13",
    }
  },
  networks: {
    development: {
      host: "127.0.0.1",
      port: 7545,
      network_id: "5777"
    }
  }
};
 