<h1>Install</h1>

<pre>
docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php82-composer \
    composer install --ignore-platform-reqs
</pre>

<h1>Running</h1>
<pre>
    alias sail=./vendor/bin/sail
    sail up -d
    sail php artisan key:generate
    sail php artisan migrate
    sail yarn install
    sail yarn run dev
</pre>

 <a href="http://localhost">localhost</a>
