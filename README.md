# Jar Ejecutable con Maven

Código fuente de ejemplo para la entrada del blog [Jar Ejecutable con Maven](https://www.hermanbarrantes.dev/jar-ejecutable-con-maven/).

## Compilación

Usando [Apache Maven Dependency Plugin](https://maven.apache.org/plugins/maven-dependency-plugin/) y [Apache Maven JAR Plugin](https://maven.apache.org/plugins/maven-jar-plugin/)

```shell
$ mvn clean package -Pmanual
$ java -jar target/example.jar
```

Usando [Apache Maven Assembly Plugin](https://maven.apache.org/plugins/maven-assembly-plugin/)

```shell
$ mvn clean package -Passembly
$ java -jar target/example-jar-with-dependencies.jar
```

Usando [Apache Maven Shade Plugin](https://maven.apache.org/plugins/maven-shade-plugin/)

```shell
$ mvn clean package -Pshade
$ java -jar target/executable-jar-maven-1.0.0-shaded.jar
```

Usando [Onejar Maven Plugin](https://github.com/jolira/onejar-maven-plugin)

```shell
$ mvn clean package -Ponejar
$ java -jar target/example-one.jar
```

