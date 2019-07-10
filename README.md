# HouseKeeping in order_Finals 2020 VIT (Udaan)

## House Keeping System

### Description

A product to solve the problem statement given during test.

In every big Organization like School, Offices, Apartment complexes, hotels e.t.c. there are number of assets that needs constant monitoring and upkeeping. Usually you would have observed that there is a specific team called house keeping that have to ensure that all assets and facilites is kept in working and usable conditions.

This product helps manage and execute the duties and various tasks of this organization.

### Install Dependencies

```
npm i
```

### Start the Server

```
node ./bin/www
```

In case of running Locally local mongo client is necessary.

## This API is Hosted at [Click Here](https://house-keeping-mehul.herokuapp.com)

API Documentation :

```
route : /add-asset
request type : POST
Body : {name : <asset_name> }
failure response : {{message : error}}
success response : {{message : success}}
```

```
route : /assets/all
request type : GET
failure response : {{message : error}}
success response : JSON of assets
```

```
route : /add-task
request type : POST
Body : {name : <task_name> ,asset : <asset_id> }
failure response : {{message : error}}
success response : {{message : success}}
```

```
route : /add-worker
request type : POST
Body : {name : <worker_name> }
failure response : {{message : error}}
success response : {{message : success}}
```

```
route : /tasks/all
request type : GET
failure response : {{message : error}}
success response : JSON of tasks
```

```
route : /workers/all
request type : GET
failure response : {{message : error}}
success response : JSON of workers
```

```
route : /get-tasks-for-worker/:id
request type : GET
failure response : {{message : error}}
success response : JSON of worker's tasks (Here id is a variable that is the object id of the worker)
```

```
route : /allocate-task
request type : POST
Body : {workerId : <worker_id>,timeOfAllocation : <timeOfAllocation>,taskId : <taskId> }
failure response : {{message : error}}
success response : {{message : success}}
```

### This API is built using Node.JS and express with MongoDB as the database and is hosted on Heroku
