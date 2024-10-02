## Laravel Testing Grounds

This is lightly modified Laravel v10 project set up using the Composer create-project command for testing in a default environment.

### Changes from Default
- Added Tailwind and Tailwind/Forms using PostCSS instead of hardcoded HTML styles.
- Switched from MYSQL to SQLite3.
- Added Livewire v3 and Laravel Livewire Tables

## Dev Setup

- Copy `.env.example` to `.env`.

- Run `php artisan key:generate`.

- Run `php artisan migrate`. If it tells you the database does not exist, accept the prompt to create one.

- Run `php artisan seed` for base test data.

- Run `php artisan serve` and `npm run dev` in separate terminals.

- Connect to `localhost:8000`.

## Specific Test Subjects

### [Laravel Livewire Tables v3](https://github.com/rappasoft/laravel-livewire-tables)

Used the `php artisan make:datatable` command to generate a table based on the default User model.

Using the manual assets import inside of app.js:
(`import '../../vendor/rappasoft/laravel-livewire-tables/resources/imports/laravel-livewire-tables-all.js';`)