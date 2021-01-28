# mern-node-todo-api

npm install

Setup mogoDB
sudo service mongod start
sudo service mongod stop
sudo service mongod status

API
#GET show
  curl -X GET \
  http://localhost:4000/todos/6012bd181c392445112a0d2a \
  -H 'cache-control: no-cache' \
  -H 'postman-token: 6cece07e-1722-bea3-e30b-d7ea0df5e7f0'

#Update
curl -X POST \
  http://localhost:4000/todos/update/6012bfb51c392445112a0d2d \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: 9c1e8b51-1aaa-1876-9727-55379176abf3' \
  -d '{
  "todo_description": "TEst",
  "todo_responsible": "Test2",
  "todo_priority": "Low",
  "todo_completed": true
}'

#GET LIST

curl -X GET \
  http://localhost:4000/todos \
  -H 'cache-control: no-cache' \
  -H 'postman-token: 5d0c74e2-9159-cd57-97fe-1d7d0edad84b'


  #create

  curl -X POST \
  http://localhost:4000/todos/add \
  -H 'cache-control: no-cache' \
  -H 'content-type: application/json' \
  -H 'postman-token: b42a54be-38f6-c063-d2ec-77d8d40e4625' \
  -d '{
  "todo_description": "TESR%6",
  "todo_responsible": "REST TEST",
  "todo_priority": "Medium",
  "todo_completed": false
}'

server run

  nodemon server