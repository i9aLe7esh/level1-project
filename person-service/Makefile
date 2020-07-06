build:
	 docker build -t person-service:v1 .
run:
	docker run --name person-container -d -p 8081:80 person-service:v1

join:
	docker exec -it person-container:v1 sh

logs:
	docker logs person-container:v1

follow:
	docker logs -f person-container:v1

stop:
	docker stop person-container:v1

clean:
	docker rm person-container:v1
