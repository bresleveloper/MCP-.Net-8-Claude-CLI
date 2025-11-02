# MCP-.Net-8-Claude-CLI

this is my attempt to build an independent .Net 8 dev env detached from my computer except local folder for whatever like source or DB.

## TODO 
* add reamde about the Dockerfile
* add reamde about the yaml file



## Instuctions:

CHANGE THE PASSWORDS FOR PRODUCTION!!


IN LOCAL FOLDER:




### build (~5 min)

* `docker-compose build` 	=> ONCE build the image
* `docker-compose up -d` 	=> run it
* `docker-compose ps` 		=> test it runs
* `docker-compose down`		=> shut down


### re-build

* `docker-compose logs` 					=> see why something was not working
* `docker-compose down -v` 					=> remove everything
* `docker rmi mcp-codernet8claude:v1.0` 	=> DELETE everything
* `docker-compose build --no-cache` 		=> rebuild without any cashing (if needed)

back to post build



## start working

* `dotnet new webapi -n TestApiSomething`			=> create an API 
* `dotnet run --urls http://0.0.0.0:8083`			=> run the api
* `http://localhost:8083/swagger/index.html`		=> see your api endpoints
* `http://localhost:8083/weatherforecast`			=> test your api




open port 8080 for coder 8083, 8094, 8105, change in yaml file