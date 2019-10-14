
## Build

Use maven to build the projects
```
mvn install
```

## Code analysis

Mhus supports sonarqube (http://sonarqube.org) to analyse the code.

Execute:
```
mvn sonar:sonar -Dsonar.host.url=http://my.server:9000/sonar -Dsonar.user=myuser -Dsonar.password=mypassword
```

## Add license headers

Mhus supports automatic update of license headers.

It's recommended to copy the file 'LICENSE_HEADER' in each project home directory.

Execute:
```
mvn license:format
```

## Format sources

You can use the google source formatter to format the source code.

Execute:
```
mvn git-code-format:format-code
```
To format the sources.
