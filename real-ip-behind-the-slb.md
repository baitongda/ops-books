# NGINX 禁用

```
http {
    real_ip_header X-Forwarded-For;
    set_real_ip_from 0.0.0.0/0;
}
```



