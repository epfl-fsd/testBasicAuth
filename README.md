# testBasicAuth

This is a "[docker-compose]" project that put [traefik] with a [basic auth] as a 
reverse proxy in front of a HelloWorld [Express] app.

## Notes

We first tryed with [nginx], but our objectif was to be able to use env vars or
secrets to define the ".htpasswd" on the fly — we weren't able to find a way to
do it with nginx while it was pretty straight forward with traefik. The nginx
service is commented in the [docker-compose.yml](./docker-compose.yml) file, feel free to test it again.


[docker-compose]: https://docs.docker.com/compose/compose-file/
[basic auth]: https://en.wikipedia.org/wiki/Basic_access_authentication
[traefik]: https://traefik.io
[Express]: https://expressjs.com/
[nginx]: https://www.nginx.com/