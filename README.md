This is the m2eclipse-core repository

- removed slf4j.api hard version constraint "1.6.2"
- replaced org.slf4j.api with official slf4j.api Bundle-SymbolicName

This will allow using m2e plugin within a juno/kepler rcp application and using a more up to date slf4j package.

Build:
 ```
 mvn -f m2e-maven-runtime clean install
 mvn clean install
 mvn update-site-p2-metadata
 ```
 
 Use org.eclipse.m2e.site/target/org.eclipse.m2e.site.1.4.2.zip as repository for your rcp app.
 