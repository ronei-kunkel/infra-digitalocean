# Environments

## Production

### build

`docker build --rm -t nginxphp82 .`

### run

`docker run -d -v $(pwd):/infra -w /infra -p 80:80 --name nginxphp82-apps nginxphp82`

## Development

### make .env file

`cp .env.example .env`

### build

`docker-compose build`

### run

`docker-compose up -d`
