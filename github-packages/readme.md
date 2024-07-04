export GH_USERNAME='jojgrev'

GH_IMAGE_NAME='hello-world'
export GH_ver='1.0.0'

echo $GH_TOKEN | docker login ghcr.io -u $GH_USERNAME --password-stdin

docker tag hello-world:latest ghcr.io/jojogrev/hello-world:1.0.0

docker push ghcr.io/jojogrev/hello-world:1.0.0