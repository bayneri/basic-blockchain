# basic blockchain

This is a basic blockchain implementation written in python. API structure is created with Python Flask Framework. 

This project is based on a [tutorial](https://hackernoon.com/learn-blockchains-by-building-one-117428612f46).

## Installation

1. Make sure [Python 3.6+](https://www.python.org/downloads/) is installed. 
2. Install [pipenv](https://github.com/kennethreitz/pipenv). 

```
$ pip install pipenv 
```

3. Create a _virtual environment_ and specify the Python version to use. 

```
$ pipenv --python=python3.6
```

4. Install requirements.  

```
$ pipenv install 
``` 

5. Run the server:
```
$ pipenv run python blockchain.py
```

## Endpoints

1. ```/mine``` to tell our server to mine a new block. **_[GET]_**
2. ```/transactions/new``` to create a new transaction to a block **_[POST]_**
3. ```/chain``` to return the full Blockchain. **_[GET]_**
4. ```/nodes/register``` to accept a list of new nodes in the form of URLs. **_[POST]_**
5. ```/nodes/resolve``` to implement our Consensus Algorithm, which resolves any conflicts—to ensure a node has the correct chain. **_[GET]_**