# 负载均衡背后的真实 IP 地址

nginx.conf

```
http {
    real_ip_header X-Forwarded-For;
    set_real_ip_from 0.0.0.0/0;
}
```

禁用 IP

```
location / {
  deny x.x.x.x;
}
```



