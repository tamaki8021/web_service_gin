```
/albums
  GET – Get a list of all albums, returned as JSON.
  POST – Add a new album from request data sent as JSON.

/albums/:id
  GET – Get an album by its ID, returning the album data as JSON.
```

https://golang.org/doc/tutorial/web-service-gin

# command

```
// POST
$ curl http://localhost:8080/albums \
    --include \
    --header "Content-Type: application/json" \
    --request "POST" \
    --data '{"id": "4","title": "The Modern Sound of Betty Carter","artist": "Betty Carter","price": 49.99}'

// GET
$ curl http://localhost:8080/albums \
    --header "Content-Type: application/json" \
    --request "GET"
```