Orienteering Backend Project
===============================

El objetivo de este proyecto es ayudarme a iniciarme con distintas tecnologías backend que no manejo aún, como Spring Boot.
Utilizaré también el framework Spock para hacer especificaciones de las funcionalidades que vaya incorporando al proyecto.

El proyecto , Gradle, etc... con The purpose of this project is to help you get started with Spock. The project includes several example specifications and build scripts for Ant, Gradle, and Maven. It also makes it easy to create an Eclipse or IDEA project, allowing you to run the example specs from within your IDE.
All three builds (Ant, Gradle, Maven) will automatically download all required dependencies, compile the project, and finally run the example specs. The Gradle build goes one step further by bootstrapping itself, alleviating the need to have a build tool preinstalled.

Requisitos previos
-------------
- JDK 5 or higher
- Maven 3.x (for Maven build)

Construir con Gradle
--------------------
Escribir: ./gradlew clean test

Los ficheros descargados (incluída la distribución de Gradle) se almacenará en el directorio local de Gradle (generalmente "<user_home>/.gradle").

Construir con Maven
-------------------
Escribir: mvn clean test

Los ficheros descargados se almacenarán en el repositorio local de Maven (generalmente "<user_home>/.m2/repository").

Crear un proyecto en Eclipse
---------------------------
Con Gradle, escribimos: ./gradlew cleanEclipse eclipse

Hay que estar seguros que tenemos la versión más reciente del plugin de Groovy para Eclipse instalado en el IDE. Después de importar el proyecto generado en un workspace, vamos a Preferences->Java->Build Path->Classpath Variables y añadimos la variable GRADLE_CACHE con el valor "<user_home>/.gradle/cache". (Si tienes establecida la variable de entorno GRADLE_USER_HOME, el valor correcto sería "<GRADLE_USER_HOME>/cache"). Después de esto, deberías ser capaz de construir el proyecto.

Crear un proyecto en IDEA
---------------------------
Type: ./gradlew cleanIdea idea

Abrir el proyecto generado en IDEA. Después de esto, deberías ser capaz de construir el proyecto.

Getting hold of the Jars used in this project
---------------------------------------------
Type: ./gradlew collectJars

The Jars will be copied to build/output/lib. The comments in build.gradle explain what they are needed for.

Further Resources
-----------------
Spock homepage        http://spockframework.org
Spock web console     http://meet.spockframework.org
Main documentation    http://wiki.spockframework.org/SpockBasics
User discussion group http://forum.spockframework.org
Dev discussion group  http://dev.forum.spockframework.org
Issue tracker         http://issues.spockframework.org
Build server          http://builds.spockframework.org
Maven repository      http://m2repo.spockframework.org (releases are also available from Maven Central)
Spock blog            http://blog.spockframework.org
Spock on Twitter      http://twitter.com/pniederw

Gradle homepage http://www.gradle.org
Groovy homepage http://groovy.codehaus.org
Maven homepage  http://maven.apache.org
