.PHONY: all build clean deploy test

build:
	env GOOS=linux go build -ldflags="-s -w" -o ./bin/hello ./main.go

clean:
	rm -rf ./bin

deploy: clean build
	sls deploy --verbose
