install: build
	docker network create postfixadmin
	docker-compose up -d
build: wipe
	docker build	-t="postfixadmin" .
wipe:
	docker-compose down
	docker network rm postfixadmin
stop:
	docker-compose stop
remove:
	docker-compose rm
