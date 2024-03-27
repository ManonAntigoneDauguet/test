# DragonManual-Back

This repo contains all the source code to run the API for DragonManual.


## 1. How to Install and Run the Project

## 1.1 Prerequisites

 - [Docker Desktop](https://www.docker.com/products/docker-desktop)


## 1.2 Installation

 - The `docker run --name dragonmanual-container -e POSTGRES_USER='User' -e POSTGRES_PASSWORD='Password' -e POSTGRES_DB=projectdatabase -p 5432:5432 -d postgres` command, with 'User' and 'Password' replaced by your own user name and password, will allow you to create your Docker container, it database and run your image on port 5432.
 - Save your user name and password in a .env file, as the .env.exemple (be carful to update the DATABASE_URL to).
 - The `npm install` command will allow you to install the dependencies.
 - The `npm run migrate up` command will allow you to migrate the database.

** Database content
If you want to fill the database with the dragon species (approximately 20), use the `npm run fill-db` command after the migration.


## 1.3 Run

 - The `npm start` command will allow to run the app in the development mode.
 - Please enjoy !