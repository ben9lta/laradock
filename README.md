<h1>Install</h1>

<pre>
docker run --rm \
    -u "$(id -u):$(id -g)" \
    -v $(pwd):/var/www/html \
    -w /var/www/html \
    laravelsail/php82-composer \
    composer install --ignore-platform-reqs
</pre>
