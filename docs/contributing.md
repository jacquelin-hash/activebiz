# Contributing
>
> ([back-home](./../README.md))

## Setting up the Development Environment

1. Clone the repository
2. Install dependencies
3. Configure the .env file
4. Create the database tables
5. Run the app

```bash
# Clone the repository
git clone git@github.com:jacquelin-hash/activebiz.git
cd activebiz

# Install dependencies
npm install && composer install

# Configure the .env file
cp .env.example .env
php artisan key:generate # Generate an app encryption key
touch database/database.sqlite # Create the sqlite database

# Create the database tables
php artisan migrate

# Run the app
npm run dev
php artisan serve

# Run the tests
./vendor/bin/phpunit tests/Feature
./vendor/bin/phpunit tests/Unit
```
