
For DEV build
docker build -f Dockerfile.dev .


For Production

docker build .
docker run -p 8080:80 <image-id>