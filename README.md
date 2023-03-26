# EmailScheduler

Email Scheduler

Email Scheduler is a web application that allows users to schedule emails to be sent at a later time. It is built using Python Flask and Firebase.

Table of Contents
Installation
Usage
Contributing
License
Installation
To install and run Email Scheduler locally, follow these steps:

Clone this repository:

bash

Copy code
git clone https://github.com/zpmughal/EmailScheduler.git

Install the required dependencies using pip:

bash
Copy code
pip install -r requirements.txt

Set up a Firebase project and configure the necessary credentials. You can follow the instructions provided in the Firebase documentation.

Create a file named config.py and add your Firebase project credentials:

python
Copy code
import os

class Config(object):
    SECRET_KEY = os.environ.get('SECRET_KEY') or 'your-secret-key'
    FIREBASE_CONFIG = {
        'apiKey': 'your-api-key',
        'authDomain': 'your-auth-domain',
        'databaseURL': 'your-database-url',
        'projectId': 'your-project-id',
        'storageBucket': 'your-storage-bucket',
        'messagingSenderId': 'your-messaging-sender-id',
        'appId': 'your-app-id',
        'measurementId': 'your-measurement-id'
    }

Run the Flask application:

bash
Copy code
export FLASK_APP=app.py
export FLASK_ENV=development
flask run

Usage

To use Email Scheduler, simply navigate to the web application at http://localhost:5000 in your web browser.

You can create a new account by clicking on the "Sign Up" button and filling out the necessary information. Once you are logged in, you can create a new email by clicking on the "New Email" button and filling out the necessary fields. You can then schedule the email to be sent at a later time by selecting the desired date and time.

You can view your scheduled emails by clicking on the "Scheduled Emails" button. You can edit or delete a scheduled email by clicking on the corresponding buttons.

Contributing

We welcome contributions to Email Scheduler. To contribute, follow these steps:

Fork this repository.

Create a new branch: git checkout -b my-new-feature.

Make changes and commit them: git commit -am 'Add new feature'.
Push to the remote branch: git push origin my-new-feature.
Create a pull request.

License

Email Scheduler is licensed under the MIT License. See LICENSE for more information.
