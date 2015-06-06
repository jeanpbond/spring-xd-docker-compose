# Simple distributed mode

Using docker-compose to run the containers :
	
	cd spring-xd-distributed-mode
    docker-compose up -d
	

To connect to the running admin server, use the springxd/shell container : 

	docker run --name shell -it shell/bin/xd-shell
    xd:>admin config server http://dockerhost:9393
	
dockerhost must be replace by your host running docker.
