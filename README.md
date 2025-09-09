# BUILD
```bash
    docker compose build
```
# RUN
```bash
    docker compose up
```
# INTSALL COMPOSER
```bash
    docker compose exec api composer install
```
# CREATE ENV FILE
```bash
    cp ./backend/.env.example ./backend/.env
```
# GENERATE API KEY
```bash
    docker compose exec api php artisan key:generate
```