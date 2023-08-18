# Tensorflow

> Tensorflow is an open-source library for machine learning developed by Google.


- Deploy the application 
```
$ playground catalog deploy napptive/tensorflow:nightly-jupyter
```

- Check if the application is ready checking the status:

```
$ playground apps info tensorflow
NAME          STATUS
tensorflow    APP_OK

COMPONENT     STATUS    SCOPES    TRAITS
tensorflow    OK                  tensorflow-ingress

COMPONENT     INGRESSES
tensorflow    tensorflow-<username>.apps.playground.napptive.dev
```

- if the application is APP_OK, copy the ingress link in your browser. 
  
- We need a token to log into the page. We can obtain the token checking the application logs:

```
$ playground apps logs tensorflow
...
 playground apps logs tensorflow
...
[tensorflow-...]    [tensorflow]    2021-05-07T14:13:20.552263379Z      or http://127.0.0.1:8888/?token=<token>
...
```

- Copy the token and paste it to log into tensorflow page