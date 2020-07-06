build:
	 docker build -t person-service:v1 .
run:
	docker run --name person-container -d -p 8081:80 person-service:v1

join:
	docker exec -it person-service:v1 sh

logs:
	docker logs person-service:v1

follow:
	docker logs -f person-service:v1

stop:
	docker stop person-service:v1

clean:
	docker rm person-service:v1
