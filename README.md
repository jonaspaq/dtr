# Online DTR
Online Daily Time Report

## Required
[Docker Desktop](https://www.docker.com/products/docker-desktop)

# Installation 🕶

Clone this repository

```
git clone https://github.com/jonaspaq/dtr.git
```

Navigate to project directory and copy env

```
cp .env.example .env
```

Build and run docker 
```
docker-compose up -d --build
```

After build, check logs if dependencies are installing. Wait for installs to succeed.

For composer, run ``` docker-compose logs -f composer ```

For npm, run ``` docker-compose logs -f node ```

# Usage 🛠
There are two projects in this repo, the backend and the frontend.

## Backend 🕹
> Note: docker-compose should be up already and dependecies should be installed successfully by now

Enter backend container
```
docker-compose exec php sh
```

Copy environment variables
```
cp .env.example
```

Generate key for project
```
php artisan key:generate
```

If you followed instructions carefully, you can visit [localhost:8000](http://localhost:8000) by now with no errors.

## Frontend 🖥
> Note: docker-compose should be up already and dependecies should be installed successfully by now

Enter frontend container
```
docker-compose exec node sh
```

Next, watch files for development
```
yarn watch
```

If you followed instructions carefully, you can visit [localhost:10080](http://localhost:10080) by now with no errors.

# Production
Coming soon.
