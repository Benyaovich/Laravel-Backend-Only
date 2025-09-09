# BUILD
```bash
    docker compose build
```
# CREATE ENV FILE
```bash
    cp ./backend/.env.example ./backend/.env
```
# RUN
```bash
    docker compose up
```
# INTSALL COMPOSER
```bash
    docker compose exec api composer install
```
# GENERATE API KEY
```bash
    docker compose exec api php artisan key:generate
```
