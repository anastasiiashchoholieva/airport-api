# Airport API - AirGate

***

API service for airport management written on DRF
## Installing using GitHub

***
Install PostgresSQL and create db

This project uses environment variables for configuration. To set up the required variables, follow these steps:

1. Create a new `.env` file in the root directory of the project.

2. Copy the contents of the `.env_sample` file into `.env`.

3. Replace the placeholder values in the `.env` file with the actual values specific to your environment.

```python
git clone https://github.com/anastasiiashchoholieva/airport-api.git
cd airport_api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```


## Run with docker
```
docker-compose up --build
```
You can use this admin user

Email: `admin@admin.com`
Password: `1qazcde3`

or 

***
- create user via /api/user/register/
***

and then generate access token:

- get access token via /api/user/token/

## Features
***
- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating routes with source and destination
- Creating airplanes
- Adding flights
- Filtering routes and flights


## Documentation

 ---

 * api/doc/swagger/: Documentation using Swagger

![doc_api.png](documentation_image%2Fdoc_api.png)