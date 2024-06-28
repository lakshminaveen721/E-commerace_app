# E-commerace_app

How to Run the Project
- Set Up Environment: Install the required packages using pip.

pip install Flask Flask-SQLAlchemy Flask-Migrate Flask-Login Flask-WTF

- Initialize the Database: Set up the database and apply migrations.

flask db init
flask db migrate -m "Initial migration."
flask db upgrade

- Run the Application: Start the Flask development server.

flask run

- Project Structure
app.py: The main application file that sets up the Flask app and defines routes for user authentication, product display, and cart operations.

config.py: Configuration file for setting up database connections and other app settings.

models.py: Defines the database models for users, products, categories, and cart items using SQLAlchemy.

forms.py: Defines the forms for user registration, login, and adding products to the cart using Flask-WTF.

templates/: Contains HTML templates for rendering the web pages.
  base.html: Base template with common layout and navigation.
  login.html: Template for the login page.
  register.html: Template for the registration page.
  products.html: Template for displaying products.
  cart.html: Template for displaying the shopping cart.

static/: Contains static files like CSS.
  styles.css: CSS file for styling the application.

migrations/: Directory for database migrations managed by Flask-Migrate.
