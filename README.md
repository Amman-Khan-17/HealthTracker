# HealthTracker
Groupmates Contributions :
Amman Ahmed Khan - Development & Dockerization of the Web App
Sameed Asif      - Testing using postman API
Asim Ayub        - Readme.md file & Documentation


Purpose of the Application :
This web application allows users to track their daily health metrics, including exercise, meditation, and sleep. It helps users maintain a healthy lifestyle by storing and visualizing their daily health data over time.


How to Build and Run the Application Using Docker :
Following commands were used.
Building the docket Image :  docker build -t health-data-tracker .
Run the Docker Container:    docker run -p 5000:5000 \ --env POSTGRES_URL=sqlite:///health_data.db \ --env SECRET_KEY=mysecretkey123 \health-tracker


Specific Environment Variables or Configurations Needed:
SECRET_KEY: A secret key for Flask session management.
POSTGRES_URL: The URL for connecting to a PostgreSQL database.

Steps for testing :

We used postman API for testing all our endpoints . A detailed evidence and step by step testing
process with screenshots is included in documentation (word file.) 

Requirements : 
requests>=2.28
Flask==2.0.3
Flask-SQLAlchemy==2.5.1
Flask-WTF==0.15.1
werkzeug==2.0.3
email-validator==2.1.1
SQLAlchemy==1.3.24
Flask-Chartjs==0.1.dev1
gunicorn
WTForms~=3.2.1
