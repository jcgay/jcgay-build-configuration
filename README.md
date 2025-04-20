Maven configuration to get binaries deploy to Maven central.

[Sonatype guide](https://central.sonatype.org/publish/publish-portal-maven/)  

To release a project:

    mvn release:prepare release:perform
    
Binaries will be deployed on Maven Central.

Authentication configuration in `settings.xml`:

	<server>
        <id>central</id>
        <username>***</username>
        <password>***</password>
    </server>
    <server>
        <id>gpg.passphrase</id>
        <passphrase>***</passphrase>
    </server>