# django_crud_app

To run this application , you need the following

  - Postgres
  - Pychamr/VsCode (any other IDE)

Steps to follow:
  - Clone this repo
  - Create a virtual env using command " python -m venv 'project name'"
  - pip install psycopg2 or psycopg( if needed )
  - make sure u have dganjo installled ( If you are using Pycharm just create a new django project and paste the folders of the repo in it accordingly)
  - now create the database , simply go to the postgres terminal or pgadmin  and create one with any name (e.g my_db).
  - In order to access the said database from the application go to the 'settings.py' file and look for the 'DATABASES'
  - Here you can edit your database credentials accordingly ( make sure t provide the correct username ,password and that the database is already created before moving ahead).
  - Run command 'python manage.py makemigrations' to prep the models (tables) to be exported. 
  - Then run " python manage.py migrate' to export the models to the database ( you must have atleast 11 tables registered in the database)
  - Finally run command "python manage.py runserver"
  - Check the browser at http://127.0.0.1:8000/
