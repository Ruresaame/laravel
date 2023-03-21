## Run Docker
Following the instructions here: https://hub.docker.com/r/bitnami/laravel
1. Create ~/User/Documents/GitHub/myapp
2. Run in command line: cd /myapp
2. Download and save https://raw.githubusercontent.com/bitnami/containers/main/bitnami/laravel/docker-compose.yml in active folder
3. Open docker-compose.yml and add a database password for production purposes and double-check all other config settings before the next step.
4. Run in command line: docker-compose up
5. Once it's ready, access http://localhost:8000 where you will see Laravel documentation.

## Install Composer Reqs For Breeze & Blade
Following the instructions here: https://laravel.com/docs/10.x/starter-kits#breeze-and-blade
1. Run in command line: docker-compose exec myapp composer require laravel/breeze --dev
2. Run in command line: docker-compose exec myapp php artisan migrate
3. Run in command line: docker-compose exec myapp npm install
4. Run in command line: docker-compose exec myapp npm run dev
5. Now access http://localhost:8000 and check in the upper right for Login and Register links. http://localhost:8000/register should now display a login/register form.

## Copy customized dashboard into project folder
Download the repository https://github.com/Ruresaame/laravel into the local project folder

## Register A New User
Access http://localhost:8000/register to enter a new user.
Once registered, you will be logged in.
See the user dashboard page for further instructions.
