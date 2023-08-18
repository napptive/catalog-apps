# Nginx Application

> Nginx web server

## References
* https://www.nginx.com/

After deploy nginx, ask for application info to know its endpoint executing:

```
$ playground apps info nginx-app
NAME         STATUS
nginx-app    APP_OK

COMPONENT    STATUS    SCOPES    TRAITS
nginx        OK                  nginx-ingress

COMPONENT    INGRESSES
nginx        nginx-<username>.apps.playground.napptive.dev
```