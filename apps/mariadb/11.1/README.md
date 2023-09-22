# MariaDB

MariaDB is one of the most popular open source relational database.


## The application

The catalog application creates a Secret with the users credentials, It is recommended to change it.

```yaml
    - name: mariadb-entities
      type: k8s-objects # Set to k8s-objects
      properties:
        objects:
          # set the k8s manifest
          # Secret
          - apiVersion: v1
            kind: Secret
            metadata:
              name: mariadb-secret
            type: Opaque
            data:
              MARIADB_USER: bWFyaWFkYnVzZXI= # user <base64>
              MARIADB_PASSWORD: cGFzc3dvcmQ= # password <base64>
              MARIADB_ROOT_PASSWORD: cGFzc3dvcmQ= # root password <base64>
          # ConfigMap
          - apiVersion: v1
            kind: ConfigMap
            metadata:
              name: mariadb-cm
            data:
              MARIADB_DATABASE: db # database name
```

The application uses a persistent volume to persists the data. This trait should be commented if your account has no 
persistent volume allowed.

```yaml
traits:
- type: storage
  properties:
    pvc:
      - name: pvc-test
        mountOnly: false
        mountPath: "/var/lib/mysql"
        resources:
          requests:
            storage: 500Mi
```

