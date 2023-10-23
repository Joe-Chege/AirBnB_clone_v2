# HBNB Flask Web Application

## Description

This project involves the use of the Flask web framework. It includes multiple scripts (`0-hello_route.py`, `1-hbnb_route.py`, `2-c_route.py`, `3-python_route.py`, `4-number_route.py`, `5-number_template.py`, `6-number_odd_or_even.py`, `7-states_list.py`, `8-cities_by_states.py`, `9-states.py`, `10-hbnb_filters.py`, `100-hbnb.py`, `101-hbnb_filters.py`, `102-hbnb.py`, `103-hbnb.py`, `104-hbnb.py`, `105-hbnb.py`, `106-hbnb.py`) that start Flask web applications with various functionalities.

## Files

| File                    | Description                                |
|-------------------------|--------------------------------------------|
| `0-hello_route.py`      | Starts a Flask web application             |
| `1-hbnb_route.py`       | Starts a Flask web application             |
| `2-c_route.py`          | Starts a Flask web application             |
| `3-python_route.py`     | Starts a Flask web application             |
| `4-number_route.py`     | Starts a Flask web application             |
| `5-number_template.py`  | Starts a Flask web application             |
| `6-number_odd_or_even.py`| Starts a Flask web application             |
| `7-states_list.py`      | Starts a Flask web application             |
| `8-cities_by_states.py` | Starts a Flask web application             |
| `9-states.py`           | Starts a Flask web application             |
| `10-hbnb_filters.py`    | Starts a Flask web application             |
| `100-hbnb.py`           | Starts a Flask web application             |
| `101-hbnb_filters.py`   | Starts a Flask web application             |
| `102-hbnb.py`           | Starts a Flask web application             |
| `103-hbnb.py`           | Starts a Flask web application             |
| `104-hbnb.py`           | Starts a Flask web application             |
| `105-hbnb.py`           | Starts a Flask web application             |
| `106-hbnb.py`           | Starts a Flask web application             |

## Author

* **Joe-Chege** - [JoeChege](https://www.linkedin.com/in/Joe-chege/)

## HBNB Flask Web Application

This repository contains a Flask web application for managing Airbnb-like listings. The application is designed to interact with a MySQL database to store and retrieve data about states, cities, amenities, and places.

## Getting Started

To get started with the HBNB Flask web application, follow the instructions below.

### Prerequisites

- Python 3.x
- Flask
- Flask SQLAlchemy
- MySQL

### Installation

1. Clone the repository to your local machine:

    ```bash
    git clone <repository-url>
    cd AirBnB_clone_v2
    ```

2. Install the required Python packages:

    ```bash
    pip install Flask Flask-SQLAlchemy
    ```

3. Set up the MySQL database using the provided `setup_mysql_dev.sql` script. Run the following command in your terminal:

    ```bash
    echo "quit" | HBNB_MYSQL_USER=hbnb_dev HBNB_MYSQL_PWD=hbnb_dev_pwd HBNB_MYSQL_HOST=localhost HBNB_MYSQL_DB=hbnb_dev_db HBNB_TYPE_STORAGE=db ./console.py
    ```

4. Load sample data into the database using the provided SQL dump:

    ```bash
    curl -o 100-dump.sql "https://s3.amazonaws.com/intranet-projects-files/holbertonschool-higher-level_programming+/290/100-hbnb.sql"
    cat 100-dump.sql | mysql -uroot -p
    ```

5. Start the Flask web application:

    ```bash
    python3 -m web_flask.100-hbnb
    ```

6. Access the application in your web browser at `http://0.0.0.0:5000/hbnb`.

## Functionality

- The web application allows users to view states, cities, amenities, and places.
- Users can filter places by states, cities, and amenities.
- The application fetches data from the MySQL database and displays it in a user-friendly interface.

## Files and Directories

- `web_flask/100-hbnb.py`: Flask application script that defines routes and renders templates.
- `web_flask/templates/100-hbnb.html`: HTML template for displaying states, cities, amenities, and places.
- `web_flask/static/styles/3-header.css`: CSS file for styling the header.
- `web_flask/static/styles/4-common.css`: CSS file for common styles.
- `web_flask/static/styles/6-filters.css`: CSS file for filter styles.
- `web_flask/static/styles/8-places.css`: CSS file for styling places.
- `web_flask/static/images/`: Directory containing images used in the application.

## Acknowledgments

This project was completed as part of the Holberton School curriculum. Special thanks to the instructors and peers for their support and guidance.

--