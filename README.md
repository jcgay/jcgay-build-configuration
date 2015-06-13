Maven configuration to get binaries deploy to Maven central.

[Sonatype guide](http://central.sonatype.org/pages/apache-maven.html)  

To release a project:

    mvn release:prepare release:perform
    
To skip nexus-oss staging deployment (same as maven-deploy-plugin using `distributionManagement`):

    mvn deploy -DskipLocalStaging