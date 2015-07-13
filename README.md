# Apache Taverna (incubating) Maven Parent pom

The Apache Taverna Maven Parent provides common build settings for the rest of
[Apache Taverna](http://taverna.incubator.apache.org/code/) (incubating).

## Prerequisites

- [JDK 7](http://www.oracle.com/technetwork/java/javase/downloads/) / [OpenJDK 7](http://openjdk.java.net/) or later
- [Apache Maven](https://maven.apache.org/download.cgi) 3.2 or later


## Installing

    mvn clean install

_Note: Modules of Taverna might not use the latest version of the Taverna
Parent. This is not generally an issue, if you want to avoid its download
from [Maven Central](http://central.maven.org/maven2/org/apache/taverna/).
you may want to build the Apache Taverna Parent version corresponding to
`<parent>` in the module's `pom.xml`_


## Details

- Version number of common dependencies are declared within `<properties>`.
- Common plugins are defined in `<plugins>`.
- This parent does NOT define the version of org.apache.taverna modules, that should
be done within `<properties>` of each top-level project.



## License

(c) 2010-2014 University of Manchester
(c) 2015 Apache Software Foundation

This product includes software developed at The
[Apache Software Foundation](http://www.apache.org/).

Licensed under the
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file
[LICENSE](LICENSE) for details.

The file [NOTICE](NOTICE) contain any additional attributions and
details about embedded third-party libraries and source code.


# Contribute

Please subscribe to and contact the
[dev@taverna](http://taverna.incubator.apache.org/community/lists#dev mailing list)
for any questions, suggestions and discussions about
Apache Taverna.

Bugs and feature plannings are tracked in the Jira
[Issue tracker](https://issues.apache.org/jira/browse/TAVERNA/component/12326807)
under the `TAVERNA` component _Taverna Maven parent_. Feel free
to add an issue!

To suggest changes to this source code, feel free to raise a
[GitHub pull request](https://github.com/apache/incubator-taverna-maven-parent/pulls).
Any contributions received are assumed to be covered by the [Apache License
2.0](https://www.apache.org/licenses/LICENSE-2.0). We might ask you
to sign a [Contributor License Agreement](https://www.apache.org/licenses/#clas)
before accepting a larger contribution.



## Disclaimer

Apache Taverna is an effort undergoing incubation at the
[Apache Software Foundation (ASF)](http://www.apache.org/),
sponsored by the
[Apache Incubator PMC](http://incubator.apache.org/).

Incubation is required of all newly accepted projects until a further review
indicates that the infrastructure, communications, and decision making process
have stabilized in a manner consistent with other successful ASF projects.

While incubation status is not necessarily a reflection of the completeness
or stability of the code, it does indicate that the project has yet to be
fully endorsed by the ASF.
