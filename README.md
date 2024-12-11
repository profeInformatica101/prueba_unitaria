# Comando Maven para crear un proyecto base de escritorio
## Windows
mvn -B archetype:generate -DarchetypeGroupId="maven-archetype-quickstart" -DgroupId="com.endes" -DartifactId="proyecto_escritorio"
## Linux
mvn archetype:generate \\
    -DarchetypeArtifactId=maven-archetype-quickstart \\
    -DinteractiveMode=false \\
    -DgroupId=com.endes \
    -DartifactId=proyecto_escritorio


# Dependencias
## JUNIT 5
### Nota: Comprueba tu versión de Java 
```xml
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter-api</artifactId>
        <version>5.11.3</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter-engine</artifactId>
        <version>5.11.3</version>
        <scope>test</scope>
    </dependency>

  </dependencies>
  
  <build>
  <plugins>
    <!-- Plugin compilador de Maven -->
    <plugin>
      <groupId>org.apache.maven.plugins</groupId>
      <artifactId>maven-compiler-plugin</artifactId>
      <version>3.8.1</version>
      <configuration>
        <source>17</source>
        <target>17</target>
      </configuration>
    </plugin>
  </plugins>
</build>
```
