git clone https://github.com/nijanthan0/Bankapp.git

# build the project
docker-compose build

# migrate all the migration changes
docker-compose run web python manage.py migrate

# create super user for authentication purpose
docker-compose run web python manage.py createsuperuser

docker-compose up

Use this URL for API documentation
http://127.0.0.1:8000/swagger/
