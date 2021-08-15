# Installing the WSU's simple-console-app archetype

After cloning, run the command below to install the archetype in the local catalog.


```
mvn clean install
```

After installation, use `mvn archetype:generate` to generate the project, specifying the archetype groupid, id, and version. For example:

```
mvn archetype:generate -DarchetypeCatalog=local -DarchetypeGroupId=edu.wsu -DarchetypeArtifactId=simple-console-app -DarchetypeVersion=1.0.0-SNAPSHOT -DgroupId=edu.wsu -DartifactId=myconsoleapp
```

To execute the main method:
```
mvn exec:java -Dexec.mainClass=edu.wsu.App
```

