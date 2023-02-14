# realtime-project-demo

Integrate Maven with SonarQube

get the plugin from sonarqube site
https://docs.sonarqube.org/9.6/analyzing-source-code/scanners/sonarscanner-for-maven/

copy the plugin form how to fix maven plugin and also go to this link to get the latest plugin version
https://mvnrepository.com/artifact/org.sonarsource.scanner.maven/sonar-maven-plugin

after which you go into the pom.xml file and add the plugin.

      <plugin>
        <groupId>org.sonarsource.scanner.maven</groupId>
        <artifactId>sonar-maven-plugin</artifactId>
        <version>3.9.1.2184</version>
      </plugin>

then go to sonarqube and generate a token to run the below command
mvn sonar:sonar -Dsonar.host.url=http://192.168.0.59:9000/sonarqube -Dsonar.login=8a66f6086d5bd367a639c31fcf0d19cd16fb286a
