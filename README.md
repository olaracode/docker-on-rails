# Docker on Rails

## Getting started

To run this project simple clone the repository and build the docker container.

```bash
git clone https://github.com/olaracode/docker-on-rails app_name
cd app_name
docker-compose up --build # To run and build the container
```

## Rails CLI

> To use the rails CLI you need to have the [container running](#getting-started).

### To access the rails CLI you can use the following command:

```bash
docker-compose exec web bash
```

### Creating a new scaffold:

```bash
rails g scaffold model_name attribute:type

# Example
rails g scaffold Post title:string body:text
```

After creating the scaffold you should run the db migrations

### Running the migrations:

```bash
rails db:migrate
```
