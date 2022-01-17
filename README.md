PersonalCheckstyle
==================

The CheckStyle file that I prefer to use for all of my projects


## Prerequisites

To build and publish this project to Maven central (through [Sonatype OSSRH](https://central.sonatype.org/publish/publish-guide/#SonatypeOSSMavenRepositoryUsageGuide-8a.ReleaseIt)), you must have the following installed (I usually install via [homebrew](https://brew.sh), but whatever is easiest):
* [GPG](https://central.sonatype.org/publish/requirements/gpg/) - Set up a key and password, per the instructions!
* [Maven](http://maven.apache.org)

## How To Release

1. Run the following command:
`mvn clean deploy -Dgpg.passphrase=<your gpg passphrase>`

2. Log into https://oss.sonatype.org (This is in the old system)

3. Go to "Staging Repositories", select the artifact that was deployed, and click on the "Close" button to ready for release.  Once it comes back, you can click the "Release" to make it avaiable on Maven Central.