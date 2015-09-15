Maven configuration to get binaries deploy to Maven central.

[Sonatype guide](http://central.sonatype.org/pages/apache-maven.html)  

To release a project:

    mvn release:prepare release:perform
    
Binaries will be deployed on Maven Central and Bintray.

Authentication configuration in `settings.xml`:

    <server>
        <id>bintray</id>
        <username>***</username>
        <password>***</password>
	</server>
	<server>
        <id>ossrh</id>
        <username>***</username>
        <password>***</password>
    </server>
    <server>
        <id>gpg.passphrase</id>
        <passphrase>***</passphrase>
    </server>