# Comando Maven para crear un proyecto base de escritorio
## Windows
mvn -B archetype:generate -DarchetypeGroupId="maven-archetype-quickstart" -DgroupId="com.endes" -DartifactId="proyecto_escritorio"
## Linux
mvn archetype:generate \\
    -DarchetypeArtifactId=maven-archetype-quickstart \\
    -DinteractiveMode=false \\
    -DgroupId=com.endes \
    -DartifactId=proyecto_escritorio
