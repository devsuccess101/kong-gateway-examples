# kong-gateway-examples

Một số mẫu ví dụ về cài đặt và sử dụng Kong Gateway v3.5.0:
- Kong Databaseless
- Kong PostgreSQL
- Kong Ingress

## whoami

Ứng dụng được dùng để demo với Kong trong repository này có tên là `whoami`:
- Được chạy 2 container từ image `traefik/whoami`
- Một số routes có trong ứng dụng này tham khảo trên [DockerHub](https://hub.docker.com/r/traefik/whoami)

## Kong + PostgreSQL

```bash
cd kong-postgresql
docker compose up -d
```

## Kong + Databaseless

```bash
cd kong-dbless
docker compose up -d
```

## Kong Ingress

```bash
cd kong-ingress
make kong
```
