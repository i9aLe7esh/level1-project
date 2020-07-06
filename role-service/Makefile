build:
	docker build -t role-service:v1 .
run:
	docker run --name role-container -d -p 8082:80 role-service:v1

join:
	docker exec -it role-service:v1 sh

logs:
	docker logs role-service:v1

follow:
	docker logs -f role-service:v1

stop:
	docker stop role-service:v1

clean:
	docker rm role-service:v1
