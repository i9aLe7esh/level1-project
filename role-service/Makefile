build:
	docker build -t role-service:v1 .
run:
	docker run --name role-container -d -p 8082:80 role-service:v1

join:
	docker exec -it role-container sh

logs:
	docker logs role-container

follow:
	docker logs -f role-container

stop:
	docker stop role-container

clean:
	docker rm role-container
