## 各メソッドのJSON検証方法
### index
* curl localhost:3000/tasks
### show
* curl localhost:3000/tasks/#{id}
### create
* curl -F "task[content]=#{contentの値}" -F "task[status]=#{statusの値}" localhost:3000/tasks.json
### update
* curl -X PUT -F "task[content]=#{contentの値}" -F "task[status]=#{statusの値}" localhost:3000/tasks/#{id}.json
### destroy
* curl -X DELETE localhost:3000/tasks/#{id}.json
