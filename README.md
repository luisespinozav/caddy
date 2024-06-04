# Caddy server

## 1. Edit Caddyfile
- The email must be correct
- The subdomain block can be duplicated for the required number of domains.

Example:
```
{
    email user@gmail.com
}
 
domain.com, www.domain.com {
    reverse_proxy  164.152.37.888:9001
}

shop.domain.com {
    reverse_proxy  164.152.37.888:9002
}
```

## 2. Run docker compose
```
docker compose up -d
``` 
