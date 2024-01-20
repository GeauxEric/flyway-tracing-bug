# greeting-quarkus

This project is used to reproduce a confusing behavior in quarkus.

## Running the application in dev mode

You can run your application in dev mode that enables live coding using:

```shell script
./gradlew quarkusDev
```

However, if one add `quarkus.datasource.jdbc.tracing=true` to the config, it will fail.
It is very confusing the flyway extension combined with this flag needs extra 3rd party diver.

