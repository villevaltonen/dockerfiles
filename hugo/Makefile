tag = hugo-sitebuilder:latest

dev:
	docker build -t ${tag} .

build:
	docker run -u $(id -u ${USER}):$(id -g ${USER}) -w /site -v ${PWD}:/site ${tag} /hugo

clean:
	rm -rf ./public