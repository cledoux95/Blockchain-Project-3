# Blockchain API 

Blockchain API which handles GET of the block by height and POST of any new block with a non-blank body in the request.

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. See deployment for notes on how to deploy the project on a live system.

### Prerequisites

Clone the repository to somewhere you want to work on it.

```
git clone <git url>

```


### Installing

Navigate to the directory inside terminal and then:

```
npm install

```

Then just run:

```
node app.js

```

to start the server.

Use Postman or Curl at http://localhost:8000 

## Routing

Use the following to interact with the API

### GET (Returns block)

Use this to GET the block at given height.

```
http://localhost:8000/api/block/{index}

```
set index = the desired height:

```
index = int

```
Example:

```
http://localhost:8000/api/block/5

```

```
{
    "hash": "3df18561aeb128cacb59ec38f5f21cdac0f099af37470e6eb10a7cc07ff4eb5d",
    "height": 5,
    "body": "Test Data #5",
    "time": "1549933540"
}

```

### POST (puts block in chain)

Use this to POST the block with your given body to end of chain.

```
http://localhost:8000/api/block

```
set body = your data

```
body = string

```
Example:

```
POST
http://localhost:8000/api/block/
body = 'yes'

```

```
Pushed block {
  "hash": "5795e5778ce3968a9ff7ea2466efb3f7e7d97c030cf451827c9985acc8b38e79",
  "height": 10,
  "body": {
    "yes": ""
  },
  "time": "1549938441"
} 
to the chain! 
lel.

```


## Deployment

Deploy it by rewriting and establishing the server connection to a real server lol.

## Built With

*  Udacity (lol)
* 

## Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

## Versioning

Versioning? psh.

## Authors

* **Christian Le Doux - Best guy.

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* Hat tip to Udacity
* Inspiration to Udacity
* etc to Udacity
