tag = hugo-sitebuilder:latest
name = hugo-sitebuilder

dev:
	docker build -t ${tag} .
	docker run -d -t --name ${name} -v ${PWD}:/site -w /site -p 1313:1313 ${tag}

build:
	docker exec ${name} /hugo

server:
	docker exec ${name} /hugo server --bind 0.0.0.0 --buildDrafts

clean:
	rm -rf ./public
	docker stop ${name} && docker rm ${name}