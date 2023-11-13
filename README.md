docker build -t rtxt/python-git:3.8-slim-git -f python-3.8/Dockerfile python-3.8
docker push rtxt/python-git:3.8-slim-git

docker build -t rtxt/python-git:3.8-slim-git-mtime -f python-3.8/Dockerfile.mtime python-3.8
docker push rtxt/python-git:3.8-slim-git-mtime

docker build -t rtxt/ruby-node:3.2.0-16.17.1 -t rtxt/ruby-node:latest -f ruby-node/Dockerfile.ruby-node ruby-node
docker push rtxt/ruby-node

docker build -t rtxt/ruby-app-base:3.2.0-16.17.1 -t rtxt/ruby-app-base:latest -f ruby-node/Dockerfile.app-base ruby-node
docker push rtxt/ruby-app-base
