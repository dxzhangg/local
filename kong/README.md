```
docker run --rm \
-e "KONG_DATABASE=postgres" \
-e "KONG_PG_HOST=c-postgres" \
-e "KONG_PG_USER=kong" \
-e "KONG_PG_PASSWORD=kong" \
-e "KONG_CASSANDRA_CONTACT_POINTS=c-postgres" \
kong kong migrations bootstrap
```