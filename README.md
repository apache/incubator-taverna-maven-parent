# Parent POM 

Common Maven Parent for [all the other Apache Taverna repositories](http://taverna.incubator.apache.org/code/).
 
Note that released Taverna modules might not use the same version of the parent, this is usually NOT an issue. The version number of the parent is simply an increasing integer.

Supplies version number constants for all external Taverna dependencies within `<properties>`
This parent does NOT define the version of `org.apache.taverna` modules, that should
be done within `<properties>` of each top-level project.

Adds in shared Maven build and reporting steps.  Note that many useful defaults are inherited from the
[Apache super-parent](http://central.maven.org/maven2/org/apache/apache/).

List additional `<repositories>` to be used (mainly for OSGi/Spring dependencies).

This does NOT contain a `<modules>` section so does NOT do Project Aggregation. To check out individual 
Apache Taverna repositories, see http://taverna.incubator.apache.org/download/code/


## License

Apache Taverna is distributed under the
[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
