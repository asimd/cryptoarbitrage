## How it works

In short it collects JSON from multipile different cryptocurrency markets, and goes through the results and finds the highest and lowest price for each coin. For example if the results look like this for LTC:
```javascript
ltc : {
  'bittrex' : 38.23,
  'jubi' : 39.78,
  'chbtc' : 51.8,
}
```
the script will find the the highest price (chbtc.com), lowest price (bittrex), and divide the two: 51.8/38.23 = ~1.35 (~35% profit margin) and then pushes these results to the browser. It will also find the next highest market pairs, e.g. chbtc / jubi is the second highest pair and chbtc/bittrex the third, jubi/bittrex the fourth and so on until every possible combination has been computed.



## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

Required: Node.js **^ V8.0.0** this program uses ES7 features such as async/await and requires a newer version of node.

### Installing

In a terminal write the following:

CD into the correct folder.

```shell
cd arbitrage
```

Install the required npm modules

```shell
npm install
```

To run the program

```shell
npm start
```

Go to ```localhost:3000``` to see a minimal display of the raw data

## Built and deployed with

* [Node.JS](https://nodejs.org) - For the backend
* [Azure](http://ccarbitrage.azurewebsites.net/) - hosts the backend (directly from this github repo)
* [Github Pages](https://manu354.github.io/cryptocurrency-arbitrage/) - hosts the beautiful frontend :) (gets data from hosted node instance on azure)


## Forked From

* **Manu Masson** - *Initial work* 


