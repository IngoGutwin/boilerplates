# WordPress Multisite Instances with Docker and Traefik

## This is my template for running WordPress Multisite using Docker.

It uses:

- Docker
- Docker Compose
- Traefik as a reverse proxy
- WordPress
- MySQL
- PhpMyAdmin for database administration (if not needed, remove it)

### You don't need to modify the docker-compose.yml file in the traefik folder

### You only need to modify the files in the project folders.

- Choose a project name and a name for your database, and add them to the .env file.

- Add your domain and a password.

### In the docker-compose.yml file, you only need to rename the service. This name should be unique, based on your project name

### You are now ready to go, it's as simple as that

Start by navigating to the traefik folder in the terminal using the command cd traefik and run docker-compose up -d.
You should run this command in every project folder, as Docker will handle the rest for you.
Go to your chosen domain and install WordPress.

### Adding More Instances if you want 

To add a new project:

- Create a new folder with a .env and docker-compose.yml file
- Add your data and spin it up with docker compose up -d