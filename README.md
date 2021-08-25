# Config server
Configuration server for _Puff_ microservices. 
For more information see [Spring Cloud Config](https://cloud.spring.io/spring-cloud-config/reference/html/).

Run the configuration server locally on port [8888](http://localhost:8888) with
```shell
mvn spring-boot:run -Dspring-boot.run.profiles=local
```

The repository includes a `Deploy` workflow that deploys the configuration server jar on Azure.
Azure runs the server with the `cloud` profile passing in the following env variables:
```
CONFIG_USER_NAME={Basic auth user name}
CONFIG_USER_PASSWORD={Basic auth password}
```
