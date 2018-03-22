include ../Makefile

build: ## Build docker image
	@docker build --rm \
		--cache-from $(DOCKER_IMAGE_NAME):$(TAG) \
		-t $(DOCKER_IMAGE_NAME):$(TAG) .

test:
	docker run -it --rm $(DOCKER_IMAGE_NAME):$(TAG) --version
