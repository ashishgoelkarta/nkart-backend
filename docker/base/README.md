# create docker base image

docker build -t amcart-base .





# create docker search image
docker build -t amcart-search -f docker/dev/Dockerfile .

docker run -p 8006:8005 amcart-search

