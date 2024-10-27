git clone https://github.com/nijanthan0/Bankapp.git

# build the project
docker-compose build

# migrate all the migration changes
docker-compose run bank python manage.py migrate

# create super user for authentication purpose
docker-compose run bank python manage.py createsuperuser

docker-compose up

Use this URL for API documentation
http://127.0.0.1:8000/swagger/

create access token in swagger
Add in authorization:  **Bearer <token'>**

customer is for customer profile
casa is account and transaction
user is for ops user



