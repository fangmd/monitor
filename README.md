

监控

- Grafana: 数据可视化平台
- Loki: 日志
- promtail: 日志收集，发送到 Loki




## grafana

```
docker-compose -f grafana-docker-compose.yml up -d
```

- 默认账号密码: admin/admin


## Loki + promtail

```
docker-compose -f loki-docker-compose.yml up -d
```

- `volumes/promtail`： 下的日志文件会被收集


## 被监控的 nginx 

```
docker-compose -f app-nginx-docker-compose.yml up -d
```
