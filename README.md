# redis-srvpl

Build and run interactively from source using:
```bash
docker run --rm -it $(docker build -q .)
```
Docker attaches the terminal which presents the Prolog console. The query below reports the Redis version if it successfully connects to a Redis server.
```prolog
?- redis_property(default, redis_version(A)).
A = "6.2.7" ;
false.
```
