# Contributing
>
> ([back-home](./../README.md))
>

## Table of Contents

- [Contributing](#contributing)
  - [Table of Contents](#table-of-contents)
  - [Setting up the Development Environment](#setting-up-the-development-environment)
  - [Making Changes](#making-changes)

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

([back to top](#table-of-contents))

## Making Changes

1. Clone the repository
2. Create a new branch
3. Make your changes
4. Run the tests
5. Commit your changes
6. Push your changes
7. Create a pull request
8. [Deploy to Production!](deployment.md)

```bash
# 1. Clone the repository
git clone git@github.com:jacquelin-hash/activebiz.git

# 2. Create a new branch
git checkout -b my-new-feature

# 3. Make your changes
code resources/views/index.blade.php

# 4. Run the tests
npm test

# 5. Commit your changes
git add . -u
git commit -m "Add some feature"

# 6. Push to the branch
git push origin my-new-feature
```

([back to top](#table-of-contents))
