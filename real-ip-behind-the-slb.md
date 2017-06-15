# 负载均衡背后的真实 IP 地址

```
http {
    real_ip_header X-Forwarded-For;
    set_real_ip_from 0.0.0.0/0;
}
```

禁用 IP

```
location / {
  index  index.php index.html index.htm;
  try_files $uri $uri/ /index.php?$query_string;
  deny 183.61.112.4;
}
```



