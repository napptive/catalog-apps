# MySQl

> MySQL is an open-source relational database management system

## How to use this

After deploy the application, use `mysql:3306` to connect to the database. The  password is defined by value of the environment variable `MYSQL_ROOT_PASSWORD` defined in the `properties`.

This application uses an independent persistent volume (defined in the package). After remove the application, it will be up to the user to remove the volume.

```bash
kubectl --kubeconfig <napptive-kubeconfig Path> delete pvc pvc

persistentvolumeclaim "pvc" deleted
```

## References

* [https://www.mysql.com/](https://www.mysql.com/)
