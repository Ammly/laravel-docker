# laravel-docker
Laravel docker template

## Usage

    docker-compose up -d --build app

After that completes, follow the steps from the [src/README.md](src/README.md) file to get your Laravel project added in (or create a new blank one).

The following are built for our web server, with their exposed ports detailed:

- **nginx** - `:8080`
- **mysql** - `:3306`
- **php** - `:9000`

Three additional containers are included that handle Composer, NPM, and Artisan commands *without* having to have these platforms installed on your local computer. Use the following command examples from your project root, modifying them to fit your particular use case.

- `docker-compose run --rm composer update`
- `docker-compose run --rm npm run dev`
- `docker-compose run --rm artisan migrate`
