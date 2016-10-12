.DEFAULT_GOAL := dev.run

.PHONY: dev.clean dev.build dev.run

help:
	@echo "Please use \`make <target>' where <target> is one of"
	@echo "  help                       display this help message"
	@echo "  dev.clean                  clean up docker development container and image"
	@echo "  dev.build                  rebuild docker image"
	@echo "  dev.run                    run the XBlock in the XBlock workbench"
	@echo ""

dev.clean:
	-docker rm {{cookiecutter.repo_name}}-dev
	-docker rmi {{cookiecutter.repo_name}}-dev

dev.build:
	docker build -t {{cookiecutter.repo_name}}-dev $(CURDIR)

dev.run: dev.clean dev.build
	docker run -p 8000:8000 -v $(CURDIR):/usr/local/src/{{cookiecutter.repo_name}} --name {{cookiecutter.repo_name}}-dev {{cookiecutter.repo_name}}-dev
