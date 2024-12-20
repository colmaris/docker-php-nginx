# Deploying a Docker Stack with PHP and Nginx

## Prerequisites

- Docker installed on your machine
- Docker Compose installed

## Project Structure

```
docker-php-nginx/
├── docker/
│   ├── nginx/
│   │   └── default.conf
│   └── php/
│       ├── Dockerfile
│       └── php.ini
├── docker-compose.yml
└── src/
    └── public/
        └── index.php
```

## Configuration

Put your files to serve with php and nginx in the `src` folder.

## Deployment

1. Run the following command to start the Docker services:

```sh
docker-compose up -d
```

4. Open your browser and go to `http://localhost` to see the PHP page.

### Check if containers running

`docker-compose ps`

### See logs if something wrong

`docker-compose logs`

### To go inside PHP container

`docker-compose exec php bash`

## Stopping the Services

To stop the Docker services, run the following command:

```sh
docker-compose down
```

## Conclusion

You now have a functional Docker stack with PHP and Nginx. You can start developing your PHP in production.
