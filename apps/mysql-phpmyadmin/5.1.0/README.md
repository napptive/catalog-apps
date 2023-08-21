# MySQl-PHPMyAdmin

> Application composed by tow components, Mysql database and PHPMyAdmin.
> MySQL is an open-source relational database management system and
> PHPMyAdmin is a free software tool written in PHP, intended to handle the administration of MySQL over the Web.

## References

* [https://www.mysql.com/](https://www.mysql.com/)
* [https://www.phpmyadmin.net/](https://www.phpmyadmin.net/)

After deploy the application, get the endpoint executing:

```bash
$ playground apps  info phpmiami-mysql
NAME              STATUS
phpmiami-mysql    APP_OK

COMPONENT     STATUS    SCOPES    TRAITS
mysql         OK
phpmyadmin    OK                  phpmyadmin-ingress

COMPONENT     INGRESSES
phpmyadmin    phpmyadmin-<user-name>.apps.playground.napptive.dev
```

you can open the link phpmyadmin-<user-name>.apps.playground.napptive.dev in your browser and login with the following credentials:

 ```bash
user: root
password: root
```
