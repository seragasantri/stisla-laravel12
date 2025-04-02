# Stisla Laravel 12 Admin Template

<p align="center">
<img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo">
</p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About This Project

This project integrates the beautiful [Stisla Admin Template](https://getstisla.com/) with Laravel 12. It provides a clean, modern dashboard interface that you can use as a starting point for your web applications.

## Getting Started

Follow these steps to get the project up and running on your local machine.

### Prerequisites

-   PHP 8.2 or higher
-   Composer
-   Node.js and npm
-   MySQL or another database system
-   Git

### Installation Steps

#### 1. Clone the repository

```bash
git clone https://github.com/seragasantri/stisla-laravel12.git
cd stisla-laravel12
```

#### 2. Install PHP dependencies

```bash
composer install
```

#### 3. Set up environment file

```bash
cp .env.example .env
```

Then edit the `.env` file to configure your database connection:

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=stisla_laravel12
DB_USERNAME=root
DB_PASSWORD=
```

#### 4. Generate application key

```bash
php artisan key:generate
```

#### 5. Run database migrations

```bash
php artisan migrate
```

If you want to seed the database with sample data:

```bash
php artisan db:seed
```

#### 6. Start the development server

```bash
php artisan serve
```

Your application will be available at http://localhost:8000

## Features

-   Modern admin dashboard using Stisla template
-   Laravel 12 framework
-   User authentication
-   Role-based access control
-   Responsive design
-   Clean and intuitive UI
-   Easy customization

## Project Structure

-   `/app` - Contains the core code of the application
-   `/resources/views` - Contains all the blade template files
-   `/public` - Contains all publicly accessible files
-   `/routes` - Contains all route definitions
-   `/database` - Contains migrations and seeders

## Troubleshooting

### Common Issues

-   **Permissions Issues**: Make sure storage and bootstrap/cache directories are writable

    ```bash
    chmod -R 775 storage bootstrap/cache
    ```

-   **Composer Errors**: Try updating composer

    ```bash
    composer self-update
    ```

-   **Database Connection Error**: Verify your database credentials in the .env file

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

-   [Laravel](https://laravel.com) - The web framework used
-   [Stisla Admin Template](https://getstisla.com/) - The admin template used
