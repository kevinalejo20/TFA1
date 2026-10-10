# Alejo PointFlow POS

A four-page CodeIgniter 4 Point-of-Sale foundation for the IT0049 Technical Formative Assessment 1.

## Included pages

- `/` - landing page
- `/about` - about page
- `/customers` - customer accounts using a static PHP array
- `/users` - user/staff accounts using a static PHP array

Each accounts page contains five sample records and uses `foreach` in its view to display the data. No database is required for this activity.

## Setup with XAMPP

1. Copy the `tfa1` folder into `C:/xampp/htdocs/alejo/`.
2. Start Apache in the XAMPP Control Panel.
3. Confirm `.env` contains:

   ```ini
   app.baseURL = 'http://localhost/alejo/tfa1/'
   ```

4. Open `http://localhost/alejo/tfa1/` in a browser.

The web server document root should point to the project's `public` folder. The project already has routes, controllers, views, and navigation links for all four required pages.

## Project structure

- `app/Config/Routes.php` - page routes
- `app/Controllers/Pages.php` - landing and about pages
- `app/Controllers/Customers.php` - customer static array
- `app/Controllers/Users.php` - user/staff static array
- `app/Views/` - HTML views
- `public/assets/css/style.css` - page styling
