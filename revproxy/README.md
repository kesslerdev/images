# Reverse proxy nginx

Nginx optimized for reverse proxy usage

put sites configurations in `/etc/nginx/sites-enabled/` on the container

### Sites examples

#### Proxy

```nginx
upstream navision {
    server 192.168.45.11:8080;
    keepalive 16;
}


server {
    listen   80;
    server_name  navision.mydomain.com;
    location / {
            proxy_pass         http://navision/;
            proxy_http_version 1.1;
            proxy_set_header   Connection "";
    }
}
```
