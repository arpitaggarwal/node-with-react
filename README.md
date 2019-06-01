# Steps to run an application

## Import Data from CSV to MongoDB

```
mongoimport -h ds261486.mlab.com:61486 -u arpitaggarwal -p ******  -d my-database -c jokes --file jokes.csv --fields joke --type csv
```

## Create Joke

```
$ curl -H "Content-Type: application/json" -X POST -d '{"joke": "Two donkeys are standing at a roadside"}' http://localhost:3050/jokes/add
```

## Get Joke

```
$ curl -X GET http://localhost:3050/jokes
```

## Delete Joke

```
$ curl -H "Content-Type: application/json" -X DELETE -d '{"joke": "Two donkeys are standing at a roadside"}' http://localhost:3050/jokes/delete
```
