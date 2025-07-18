# NOTE

1. Create a docker network

```
docker network create web
```

2. For Other App Labels

```
   - 'traefik.enable=true'
   - 'traefik.http.routers.app1.rule=Host(`app1.example.com`)'
   - 'traefik.http.routers.app1.entrypoints=websecure'
   - 'traefik.http.routers.app1.tls.certresolver=leresolver'
   - 'traefik.http.services.app1.loadbalancer.server.port=3000'
```
