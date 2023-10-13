# Environments

## Production

### build

`docker build --rm -t nginxphp82 .`

### run

`docker run -d -v /var/log/nginx/:/var/log/nginx/ -v $(pwd):/infra -w /infra -p 80:80 --name nginxphp82-apps nginxphp82`

### any alterations needs made inside of container

`docker exec -it nginxphp82-apps bash`

## Development

### make .env file

`cp .env.example .env`

### build

`docker-compose build`

### run

`docker-compose up -d`

### databases

If you need use any database, you need create them first if not exist
