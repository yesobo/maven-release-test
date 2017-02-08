# Push and tat in git with maven release plugin and keep release pom @ pom.nexus.xml.

execute the following command:

```
mvn release:clean && mvn release:prepare-with-pom -DdryRun && mv pom.xml.tag pom.nexus.xml && mvn release:clean && mvn release:prepare
```

Ignored files at `.gitignore` file:

- target/
- pom.xml.next
- pom.xml.releaseBackup
- pom.xml.tag
- release-pom.xml
- release.properties
- pom.nexus.xml
