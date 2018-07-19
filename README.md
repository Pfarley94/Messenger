
# install composer dependencies
composer update

# install npm dependencies
npm install

# generate a key for your application
php artisan key:generate

# add the database connection config to your .env file and fill out
DB_CONNECTION=mysql
DB_DATABASE=
DB_USERNAME=
DB_PASSWORD=

# run the migration files to generate the schema
php artisan migrate



#It is necessary to have the below in the .env file but it use is not necessary once the app is running unless you want infomation on usage.

# visit https://pusher.com and create a free app. then copy the keys into your .env file
PUSHER_APP_ID=your_pusher_app_id
PUSHER_APP_KEY=your_pusher_app_key
PUSHER_APP_SECRET=your_pusher_app_secret
PUSHER_APP_CLUSTER=your_pusher_cluster

# change the BROADCAST_DRIVER in your .env to pusher
BROADCAST_DRIVER=pusher

# run webpack and watch for changes
npm run watch
