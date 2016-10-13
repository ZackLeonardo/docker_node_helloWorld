# docker_node_helloWorld
This is a test project that develop node app in docker with DI tool--jenkins.

## Usage
1. make a Dockerfile
2. prepear the node package.json and app.js file
3. create a jenkins job

docker build -t maiz9088/docker-node-hello .

#if [docker ps -a | grep node-hello != ""]; then
  docker rm node-hello
#fi

docker run --name node-hello -d maiz9088/docker-node-hello

## License

[MIT License](http://opensource.org/licenses/mit-license.html). © Zou Deyi
