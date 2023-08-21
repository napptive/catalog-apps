# Wordpress

> Wordpress blog platform using MySQL as database.

## How to access to wordpress

Once the application has been deployed, open the public endpoint navigating through the web UI to select the application, selecting the wordpress component, and clicking on the associated Endpoint. Alternatively with the CLI use:

```
playground apps open my-wordpress
```

The wordpress instance automatically gets a public URL in the form of:

```
https://wordpress-<code>.apps.playground.napptive.dev
```

## Admin area

To access the admin dashboard, append "/admin" to the wordpress URL:

```
https://wordpress-<code>.apps.playground.napptive.dev\admin
```

The default credentials are:

* User: user
* Password: bitnami

**Note**: Please remember to change the user/password for the instance.

## References
* https://wordpress.com/
* https://www.mysql.com/