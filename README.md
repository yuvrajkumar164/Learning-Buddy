# Learning-Buddy

Initial Spring Boot application generated with Spring Initializr. The Maven
project is in `app`.

## Prerequisites

- JDK 21 with `JAVA_HOME` pointing to the JDK installation.
- Internet access for the first build to download Maven and dependencies.

The Maven Wrapper is included; a separate Maven installation is not required.

## Build and run

From the repository root in PowerShell:

```powershell
Set-Location app
.\mvnw.cmd clean verify
.\mvnw.cmd spring-boot:run
```

`clean verify` compiles the application, runs the context-load test, and creates
`app\target\app-0.0.1-SNAPSHOT.jar` (relative to the repository root).

To run the packaged application from the `app` directory:

```powershell
java -jar .\target\app-0.0.1-SNAPSHOT.jar
```

This scaffold includes the core Spring Boot starter, not a web starter. It has
no HTTP endpoints or embedded web server, so exiting after successful startup
is expected.

## First check-in

Commit the source, `pom.xml`, Maven Wrapper scripts, and
`app\.mvn\wrapper\maven-wrapper.properties`. Local IDE settings and generated
`target` output are ignored. The generated `app\HELP.md` is also intentionally
ignored by the Initializr `.gitignore`.