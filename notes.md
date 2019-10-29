
For DEV build
docker build -f Dockerfile.dev .
docker run -p 3000:3000 <image-id>

using with volumes - helps to refer the file in local - Note this doesn't work in fish terminal
docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <image-id>

For Production

docker build .
docker run -p 8080:80 <image-id>