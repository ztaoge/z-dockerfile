### create image by Dockerfile
docker build -t openrest:v1 .

### run a container
docker run -d -v $(pwd)/conf/conf.d:/etc/nginx/conf.d -p 9501:8080 -p 9502:80 openrest:v1
