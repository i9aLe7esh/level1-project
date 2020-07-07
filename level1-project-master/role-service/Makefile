build:
	docker build -t role-service:v1 .
run:
	docker run --name role-container -d -p 8082:80 role-service:v1

join:
	docker exec -it role-container:v1 sh

logs:
	docker logs role-container:v1

follow:
	docker logs -f role-container:v1

stop:
	docker stop role-container:v1

clean:
	docker rm role-container:v1
