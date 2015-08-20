# mongoose-connector
MongooseConnector loads Mongoose models from a directory and connects to a MongoDB instance.


## Installation

		$ npm install mongoose-connector

## Usage

```js
var mongoose = require('mongoose')
var MongooseConnector = require('mongoose-connector')

// Define database connection options
var opts = {
	username: 'user',
	password: 'pass',
	host: 'localhost',
	port: 27107,
	database: 'db',
	modelsFilePath: __dirname + '/models'
}

// Create the MongooseConnector object
var mc = new MongooseConector(opts);

// Connect to your database
mc.connect()

// Access your models
var User = mongoose.models('User')

```

## License
MIT
