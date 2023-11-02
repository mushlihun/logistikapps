# Manufacture Apps
Web apps using php 8 laravel

## Development
You had to following these step below for developing this application:
1. Clone this repository.
2. Create an `.env` file.
    You have to create an `.env` file based on `.env.example` file. these are some variables that need to be set.
    Database connection is required, please filling up all variables below:
    ```
    ....
    DB_CONNECTION=mysql
    DB_HOST=127.0.0.1
    DB_PORT=3306
    DB_DATABASE=senlog
    DB_USERNAME=root
    DB_PASSWORD=root
    ....
    ```
    This apps is also capale for sending emails but you have to setup the connection to the email server first. please filling up these variables:
    ```env
    MAIL_MAILER=
    MAIL_HOST=
    MAIL_PORT=
    MAIL_USERNAME=
    MAIL_PASSWORD=
    MAIL_ENCRYPTION=
    MAIL_FROM_ADDRESS=
    ```
    This apps is also capable using [Google OAuth](https://developers.google.com/identity/protocols/oauth2). First, you need create a project on [Google Cloud](https://console.cloud.google.com/projectcreate). then, [create a credentials for OAuth](https://console.developers.google.com/apis/credentials) for filling these variables.
    ```env
    ...
    GOOGLE_OAUTH_CLIENT_ID=
    GOOGLE_OAUTH_CLIENT_SECRET=
    ...
    ```
3. run the `composer install` command on terminal:
    ```bash
    composer install
    ```
4. Generate Laravel key:
    ```bash
    php artisan key:generate
    ```
5. Migrate the database:
    ```bash
    php artisan migrate
    ```
    <small>Reference: [https://laravel.com/docs/8.x/migrations#introduction](https://laravel.com/docs/8.x/migrations#introduction)</small>
6. Seed the database:
    ```bash
    php artisan db:seed
    ```
    <small>Reference: [https://laravel.com/docs/8.x/seeding#introduction](https://laravel.com/docs/8.x/seeding#introduction)</small>
7. Serve the web apps
    For quickstart you can type command below:
    ```bash
    php artisan serve
    ```
8. Initialize the apps
    This app need a few initial setup to make it works. To setting up, first, open your browser and go to `localhost/initialize-app`. then, follow the instruction to initial setup.
9. Done
    Congratulations‼, this App is ready for development. You can use credential below to login into the apps:
    
    ```
    email     : lihun@yahoo.co.id
    password  : lihun123
    ```

## Contributing

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4. Push to the Branch (`git push origin feature/AmazingFeature`).
5. Open a Pull Request.

## License

The code is released under the MIT license.

## Contact

Email - [mushlihun@live.com](mailto:mushlihun@live.com?subject=[GitHub]%20Logistik%20Apps)
