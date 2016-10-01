On Docker Hub: [rlaskey/mysql](https://hub.docker.com/r/rlaskey/mysql/).

Same as the default image, but at least so far, just set the default server
character set to utf8mb4. Why? UTF8 is a good choice for basically everything
at this point, and utf8mb4 allows for emoji, which chances are coming to your
DB whether you like it or not.
