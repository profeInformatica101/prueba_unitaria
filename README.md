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
'''xml
<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/maven-v4_0_0.xsd">
  <modelVersion>4.0.0</modelVersion>
  <groupId>com.endes</groupId>
  <artifactId>proyecto-escritorio</artifactId>
  <packaging>jar</packaging>
  <version>1.0-SNAPSHOT</version>
  <name>proyecto-escritorio</name>
  <url>http://maven.apache.org</url>
  <dependencies>

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
</project>

'''
