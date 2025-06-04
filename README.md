```markdown
# Adl-Barristers Website (CodeIgniter Project)

This is the official web application project for **Adl-Barristers**, developed using the CodeIgniter PHP framework. The site showcases legal services, team profiles, contact functionality, and more.

---

## 🛠️ Technologies Used

- **Backend:** PHP (CodeIgniter 3.x / 4.x – specify version)
- **Frontend:** HTML5, CSS3, Bootstrap, JavaScript, jQuery
- **Database:** MySQL
- **Server Requirements:**
  - PHP 7.4+ (or as per CodeIgniter version)
  - MySQL 5.7+
  - Apache/Nginx with mod_rewrite enabled

---

## 📁 Project Structure

```

/application
/controllers
/models
/views
/assets
/css
/js
/images
/system
/vendor (if using Composer)
.env (if using CodeIgniter 4)
index.php
.htaccess

````

---

## ⚙️ Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/adl-barristers.git
cd adl-barristers
````

### 2. Configure Environment

* Update the `application/config/config.php` and `application/config/database.php` files:

  ```php
  $config['base_url'] = 'http://localhost/adl-barristers/';

  $db['default'] = array(
      'hostname' => 'localhost',
      'username' => 'your_db_user',
      'password' => 'your_db_pass',
      'database' => 'adl_barristers',
      'dbdriver' => 'mysqli',
      ...
  );
  ```

### 3. Import the Database

* Import the SQL file located in the `/database/` folder (if included) via phpMyAdmin or the CLI.

```bash
mysql -u your_db_user -p adl_barristers < database/adl_barristers.sql
```

### 4. Enable `.htaccess` for Clean URLs

Make sure `mod_rewrite` is enabled on your server and that the `.htaccess` file is active in your project root.

---

## 📌 Features

* Home page with banner and service overview
* Team section with profiles of barristers
* Contact form with validation and email sending
* Practice areas with detailed descriptions
* Blog (optional)
* Admin panel to manage site content (optional, if implemented)

---

## 🧪 Development & Testing

* Use a local server (XAMPP/Laragon/WAMP) for development
* Enable `display_errors` in PHP for debugging
* Keep environment as `development` in `index.php`

```php
define('ENVIRONMENT', 'development');
```

---

## 🚀 Deployment Notes

* Point domain root to `/index.php` or set `RewriteBase /` correctly
* Change environment to `production`
* Secure `/application` and `/system` folders if possible

---

## 🤝 Credits

Developed by \[Your Name / Your Company Name]
For: **Adl-Barristers**

---

## 📬 Contact

For issues or suggestions, please contact:
📧 [info@adl-barristers.com](mailto:info@adl-barristers.com)
🌐 [www.adl-barristers.com](http://www.adl-barristers.com)

