build:
	DOCKER_BUILDKIT=1 docker build -t department-service:v1 .
run:
	docker run --name department-container -d -p 8083:80 department-service:v1

join:
	docker exec -it department-service:v1 sh

logs:
	docker logs department-service:v1

follow:
	docker logs -f department-service:v1

stop:
	docker stop department-service:v1

clean:
	docker rm department-service:v1

