# Container Observability Report

## 1. Application Logs

The `docker logs clientwebsite` command was used to retrieve the application logs from the Nginx container. The logs show three successful HTTP requests with status code 200 and one failed request with status code 404.

### 404 Error Log

```text
172.17.0.1 - - [09/Oct/2026:04:12:28 +0000] "GET /hidden-admin-page HTTP/1.1" 404 153 "-" "curl/8.5.0" "-"
```

Application logs are important because they show the requests received by the application and the errors that occurred. They help engineers identify problems, investigate failed requests, and determine what needs to be fixed.

## 2. Screenshot Evidence

* `docker-logs.png` — Nginx application logs showing successful requests and the 404 error.

