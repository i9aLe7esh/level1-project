build:
	DOCKER_BUILDKIT=1 docker build -t department-service:v1 .

run:
	docker run --name department-container -d -p 8083:80 department-service:v1

join:
	docker exec -it department-container sh

logs:
	docker logs department-container

follow:
	docker logs -f department-container

stop:
	docker stop department-container

clean:
	docker rm department-container
