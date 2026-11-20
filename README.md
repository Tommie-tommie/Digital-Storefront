# Digital-Storefront-CSC471
Basic digital storefront project for my database design class (CSC471). 
Buit  with [Laravel](https://laravel.com) 

 
> **Status:** Early development. This is the initial project scaffold.

## Requirements
 
- PHP 8.2 or newer (check `composer.json` for the exact constraint)
- Composer
- Node.js and npm
- A Postgresql database 

Required PHP extensions include `mbstring`, `xml`, `curl`, `zip`, and your database driver (e.g. `pdo_sqlite`). On Fedora:
 
```bash
sudo dnf install php-mbstring php-xml php-pdo php-zip php-sqlite3
```
 
## Getting Started
 
Clone the repository and install dependencies:
 
```bash
git clone <your-repo-url>
cd Digital-Storefront
 
composer install
npm install
```
 
Set up your environment:
 
```bash
cp .env.example .env
php artisan key:generate
```
 
If you're using SQLite, create the database file, then run migrations:
 
```bash
touch database/database.sqlite
php artisan migrate
```
 
## Running the App
 
Start the Laravel server and the Vite dev server in two terminals:
 
```bash
php artisan serve
```
 
```bash
npm run dev
```
 
Then visit <http://localhost:8000>.
 
## Building for Production
 
```bash
npm run build
```
 
## Testing and Code Quality
 
```bash
php artisan test              # run the test suite
vendor/bin/pint               # format PHP code
vendor/bin/phpstan analyse    # static analysis
```
 
## Project Structure
 
| Path | Purpose |
| --- | --- |
| `app/` | Application code (models, controllers, etc.) |
| `routes/` | Route definitions |
| `resources/` | Frontend source (JS/TS, CSS, views) |
| `database/` | Migrations, factories, seeders |
| `config/` | Configuration files |
| `tests/` | Automated tests |
| `public/` | Web root and compiled assets |
 

## License
 
This project is licensed under [GNU GPL-3.0](LICENSE).
 
