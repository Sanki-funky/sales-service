# sales-service
Sank sales recording, cancellations and transactional outbox

## Running

Run `go run ./cmd/server` from this repository. The server listens on port `8082`.

## Liveness

`GET /health/live` returns `200 OK` with an empty body. It checks that the
HTTP server can respond, not that any dependencies are ready.

```sh
curl -i http://localhost:8082/health/live
```
