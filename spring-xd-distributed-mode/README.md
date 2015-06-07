# Spring XD distributed mode

Using docker-compose to run the containers :
	
	cd spring-xd-distributed-mode
    docker-compose up -d
	
To connect to the running admin server, use the springxd/shell container. dockerhost must be replace by your host running docker : 

	docker run --name shell -it springxd/shell
    xd:>admin config server http://dockerhost:9393
	
Upon starting Spring XD, the Admin UI is available at :

	http://dockerhost:9393/admin-ui