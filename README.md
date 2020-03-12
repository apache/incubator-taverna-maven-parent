## Taverna Project Retired

> tl;dr: The Taverna code base is **no longer maintained** 
> and is provided here for archival purposes.

From 2014 till 2020 this code base was maintained by the 
[Apache Incubator](https://incubator.apache.org/) project _Apache Taverna (incubating)_
(see [web archive](https://web.archive.org/web/20200312133332/https://taverna.incubator.apache.org/)
and [podling status](https://incubator.apache.org/projects/taverna.html)).

In 2020 the Taverna community 
[voted](https://lists.apache.org/thread.html/r559e0dd047103414fbf48a6ce1bac2e17e67504c546300f2751c067c%40%3Cdev.taverna.apache.org%3E)
to **retire** Taverna as a project and withdraw the code base from the Apache Software Foundation. 

This code base remains available under the Apache License 2.0 
(see _License_ below), but is now simply called 
_Taverna_ rather than ~~Apache Taverna (incubating)~~.

While the code base is no longer actively maintained, 
Pull Requests are welcome to the 
[GitHub organization taverna](http://github.com/taverna/), 
which may infrequently be considered by remaining 
volunteer caretakers.


### Previous releases

Releases 2015-2018 during incubation at Apache Software Foundation
are available from the ASF Download Archive <http://archive.apache.org/dist/incubator/taverna/>

Releases 2014 from the University of Manchester are on BitBucket <https://bitbucket.org/taverna/>

Releases 2009-2013 from myGrid are on LaunchPad <https://launchpad.net/taverna/>

Releases 2003-2009 are on SourceForge <https://sourceforge.net/projects/taverna/files/taverna/>

Binary JARs for Taverna are available from 
Maven Central <https://repo.maven.apache.org/maven2/org/apache/taverna/>
or the myGrid Maven repository <https://repository.mygrid.org.uk/>


# Taverna Maven Parent pom

The Taverna Maven Parent provides common build settings for the rest of
[Taverna](https://web.archive.org/web/*/https://taverna.incubator.apache.org/code/).

## Prerequisites

- [JDK 8](http://www.oracle.com/technetwork/java/javase/downloads/) / [OpenJDK 8](http://openjdk.java.net/) or later
- [Apache Maven](https://maven.apache.org/download.cgi) 3.2 or later


## Installing

    mvn clean install

_Note: Modules of Taverna might not use the latest version of the Taverna
Parent. This is not generally an issue, if you want to avoid its download
from [Maven Central](http://central.maven.org/maven2/org/apache/taverna/).
you may want to build the Taverna Parent version corresponding to
`<parent>` in the module's `pom.xml`_


## Details

- Version number of common dependencies are declared within `<properties>`.
- Common plugins are defined in `<plugins>`.
- This parent does NOT define the version of org.apache.taverna modules, that should
be done within `<properties>` of each top-level project.
- Versions of dependencies that are only used within one particular project
(e.g. `beanshell.version` within `incubator-taverna-common-activities`)
should rather be defined in the top-level `pom.xml` of that project.



## License

(c) 2010-2014 University of Manchester
(c) 2014-2016 Apache Software Foundation

This product includes software developed at The
[Apache Software Foundation](http://www.apache.org/).

Licensed under the
[Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0), see the file
[LICENSE](LICENSE) for details.

The file [NOTICE](NOTICE) contain any additional attributions and
details about embedded third-party libraries and source code.


# Contribute

Any contributions received are assumed to be covered by the [Apache License
2.0](https://www.apache.org/licenses/LICENSE-2.0). 
