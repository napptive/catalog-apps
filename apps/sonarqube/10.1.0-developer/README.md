# Sonarqube

> Sonarqube is an automatic code review tool that empowers all developers to write cleaner and safer code

Once your application is up and running (it will take some minutes to be available),
check the logs and wait until the application is  up and running
```
...
... INFO  ce[][o.s.c.c.CePluginRepository] Load plugins
... INFO  ce[][o.s.c.c.ComputeEngineContainerImpl] Running Developer edition
... INFO  ce[][o.s.ce.app.CeServer] Compute Engine is started
... INFO  app[][o.s.a.SchedulerImpl] Process[ce] is up
... INFO  app[][o.s.a.SchedulerImpl] SonarQube is operational
...
```

Use _admin/admin_ credentials to log in to the application and follow the instructions to configure a project.

![Sonarqube login Screenshot](https://storage.googleapis.com/artifacts.playground.napptive.dev/logos/sonarqube/login.png)

## NOTE

_This application should be used for evaluation purpose only, the image uses an embedded H2 database and there is no persistent storage defined._

## References

* [https://www.sonarqube.org/](https://www.sonarqube.org/)
* [https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/](https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/)
* [https://hub.docker.com/_/sonarqube?tab=description](https://hub.docker.com/_/sonarqube?tab=description)
