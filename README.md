# aws-eb-python-django

An example Python/Django app which deploys to Amazon Elastic Beanstalk.


## Installation

Install the backend dependencies:

    cd backend
    pip install -r requirements.txt

Install the frontend dependencies:

    cd frontend
    npm install


## Usage

Run the backend locally using python:

    cd backend
    python manage.py runserver

Run the frontend locally using gulp:

    cd frontend
    npm start

Then visit the site at:

    http://localhost:8000/

You can access the admin CMS at:

    http://localhost:8000/admin/


## Deployment

Ensure you are in the backend folder:

    cd backend

Set your Elastic Beanstalk project by following the steps:

    eb init --profile home

Create an environment by name:

    eb create name --database

Deploy your project to Elastic Beanstalk using:

    eb deploy name
