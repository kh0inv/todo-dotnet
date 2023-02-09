### Docker

```
docker-compose up -d
```

Cần đảm bảo đã có database và sẵn sàng kết nối. Nên lần đầu chạy, container chính sẽ fail =>  chạy lại lệnh trên

### Kubernetes

```
cd deployment\helm

helm upgrade -i mypostgresql -f postgres/values.yaml bitnami/postgresql

helm upgrade -i todoapp -f todo-app/values.yaml todo-app
```
