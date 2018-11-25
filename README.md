# MyDataStack
Addressed the need for me to locally connect to mongoDb, Mysql databases and the ElasticSearch logger. Data is persisted after the [Docker] container is 'downed' or stopped.

## To install
Make sure you have [Docker] installed on your local machine.
```
docker-compose up --build
```
## To start the Docker container
```
docker-compose up
```

## To stop the Docker container
```
docker-compose down
```

## MongoDb
[MongoDB] is a free and open-source cross-platform document-oriented database program. Classified as a NoSQL database program, MongoDB uses JSON-like documents with schemata

### Connect to MongoDB 
[Robo 3T]

Address: localhost

Port: 27017

[Node.js] 

Port Forwarding (connecting from within the [Docker] container)
```
mongodb://localhost:27017/{db_name_here}
```

## Mysql
[MySQL] is an open source relational database management system.

### Connect to MySQL
* Address/Host: 127.0.0.1
* Port: 3306
* Username: root
* Password: root_password

Port Forwarding (connecting from within the [Docker] container)
```
mysql://local:local_password@localhost:3306{db_name_here}
```

## Elasticsearch
The node elasticsearch listens on localhost:9200 while elasticsearch2 talks to elasticsearch over a Docker network.

[Robo 3T]: https://robomongo.org
[MySQL]: https://www.mysql.com/
[Node.js]: https://nodejs.org
[Express]: https://expressjs.com/
[PassportJS with JWTokens]: http://www.passportjs.org/
[MongoDB]: https://www.mongodb.com/
[Docker]: https://www.docker.com/
