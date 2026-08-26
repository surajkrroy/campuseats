# HTTP Log

Public read-only JSON API used: JSONPlaceholder

## Request 1 — GET /posts/1

### Command

```powershell
curl.exe -i https://jsonplaceholder.typicode.com/posts/1
```

### Full response

```text
HTTP/1.1 200 OK
Date: Wed, 26 Aug 2026 06:10:22 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 292
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"124-yiKdLzqO5gfBrJFrcdJ8Yq0LGnU"
expires: -1
nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600,"success_fraction":0.01,"failure_fraction":0.1}
pragma: no-cache
report-to: {"group":"heroku-nel","endpoints":[{"url":"https://nel.heroku.com/reports?s=PD3aZ5JXmnXLLbuM9yuy2jwg6ke8U5C2Yq%2BT0erzkj0%3D\u0026sid=e11707d5-02a7-43ef-b45e-2cf4d2036f7d\u0026ts=1775729378"}],"max_age":3600}
reporting-endpoints: heroku-nel="heroku-nel"
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 730
x-ratelimit-reset: 1775729393
Age: 10051
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a310ac478ef13dc9-SIN
alt-svc: h3=":443"; ma=86400

{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati excepturi optio reprehenderit",
  "body": "quia et suscipit\nsuscipit recusandae consequuntur expedita et cum\nreprehenderit molestiae ut ut quas totam\nnostrum rerum est autem sunt rem eveniet architecto"
}
```

### Annotation

- `200 OK` means the request was successful.
- `Content-Type: application/json` means the response body is JSON.

## Request 2 — GET /posts/9999 (deliberate 404)

### Command

```powershell
curl.exe -i https://jsonplaceholder.typicode.com/posts/9999
```

### Full response

```text
HTTP/1.1 404 Not Found
Date: Wed, 26 Aug 2026 09:24:21 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 2
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"2-vyGp6PvFo4RvsFtPoIWeCReyIC8"
expires: -1
nel: {"report_to":"heroku-nel","response_headers":["Via"],"max_age":3600}
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 997
x-ratelimit-reset: 1787721937
Age: 14339
cf-cache-status: HIT
CF-RAY: a311c8732e2a3e5b-SIN
alt-svc: h3=":443"; ma=86400

{}
```

### Annotation

- `404 Not Found` means the requested resource was not found.
- `Content-Type: application/json` means the response body is JSON.

## Request 3 — GET /users/1

### Command

```powershell
curl.exe -i https://jsonplaceholder.typicode.com/users/1
```

### Full response

```text
HTTP/1.1 200 OK
Date: Wed, 26 Aug 2026 09:25:13 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 509
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"1fd-+2Y3G3w049iSZtw5t1mzSnunngE"
expires: -1
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 840
x-ratelimit-reset: 1787597880
Age: 23216
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a311c9b6ca0ffd1c-SIN
alt-svc: h3=":443"; ma=86400

{
  "id": 1,
  "name": "Leanne Graham",
  "username": "Bret",
  "email": "Sincere@april.biz",
  "address": {
    "street": "Kulas Light",
    "suite": "Apt. 556",
    "city": "Gwenborough",
    "zipcode": "92998-3874",
    "geo": {
      "lat": "-37.3159",
      "lng": "81.1496"
    }
  },
  "phone": "1-770-736-8031 x56442",
  "website": "hildegard.org",
  "company": {
    "name": "Romaguera-Crona",
    "catchPhrase": "Multi-layered client-server neural-net",
    "bs": "harness real-time e-markets"
  }
}
```

### Annotation

- `200 OK` means the request was successful.
- `Content-Type: application/json` means the response body is JSON.

## Request 4 — GET /todos/1

### Command

```powershell
curl.exe -i https://jsonplaceholder.typicode.com/todos/1
```

### Full response

```text
HTTP/1.1 200 OK
Date: Wed, 26 Aug 2026 09:47:22 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 83
Connection: keep-alive
cache-control: max-age=43200
etag: W/"53-hfEnumeNh6YirfjyjaujcOPPT+s"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
x-ratelimit-reset: 1786063423
Age: 3
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a311ea26e9e6a2c5-SIN
alt-svc: h3=":443"; ma=86400

{
  "userId": 1,
  "id": 1,
  "title": "delectus aut autem",
  "completed": false
}
```

### Annotation

- `200 OK` means the request was successful.
- `Content-Type: application/json` means the response body is JSON.

## Request 5 — GET /comments/1

### Command

```powershell
curl.exe -i https://jsonplaceholder.typicode.com/comments/1
```

### Full response

```text
HTTP/1.1 200 OK
Date: Wed, 26 Aug 2026 09:48:20 GMT
Content-Type: application/json; charset=utf-8
Content-Length: 268
Connection: keep-alive
access-control-allow-credentials: true
Cache-Control: max-age=43200
etag: W/"10c-KJ4I9RM/+33TKdV8CFsIvqsDSP0"
expires: -1
pragma: no-cache
Server: cloudflare
vary: Origin, Accept-Encoding
via: 2.0 heroku-router
x-content-type-options: nosniff
x-powered-by: Express
x-ratelimit-limit: 1000
x-ratelimit-remaining: 999
x-ratelimit-reset: 1787733817
Age: 3938
Accept-Ranges: bytes
cf-cache-status: HIT
CF-RAY: a311eb918b13ce29-SIN
alt-svc: h3=":443"; ma=86400

{
  "postId": 1,
  "id": 1,
  "name": "id labore ex et quam laborum",
  "email": "Eliseo@gardner.biz",
  "body": "laudantium enim quasi est quidem magnam voluptate ipsam eos\ntempora quo necessitatibus\ndolor quam autem quasi\nreiciendis et nam sapiente accusantium"
}
```

### Annotation

- `200 OK` means the request was successful.
- `Content-Type: application/json` means the response body is JSON.
