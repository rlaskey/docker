On Docker Hub: [rlaskey/php-composer](https://hub.docker.com/r/rlaskey/php-composer/).

Start w/ PHP 7, then add Composer. Here are some ways you could run it:

```
docker run -it --rm rlaskey/php-composer
docker run -it --rm -v "$PWD":/srv -w /srv rlaskey/php-composer composer install
docker run -it --rm -v "$PWD":/srv -w /srv rlaskey/php-composer vendor/bin/phpunit
```

Please extend / fork to taste.

Re: Docker running as root, you'll see a scary message warning against such a
thing. I wouldn't worry about it, though, as it's only root within the
container. If someone knows how to keep that from popping up, please file a
GitHub issue.
