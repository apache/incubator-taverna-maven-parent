# Parent POM 


Common Maven Parent for [all the other Apache Taverna repositories](http://taverna.incubator.apache.org/code/).
 
Note that released Taverna modules might not use the same version of the parent, this is usually NOT an issue.


Supplies Version number constants for all external Taverna dependencies.  

Adds in shared Maven build and reporting steps.  

List additional repositories to be used (mainly for OSGi/Spring dependencies).

This does NOT contain a `<modules>` section so does NOT do Project Aggregation.

This parent does NOT define the version of org.apache.taverna modules, that should
be done within `<properties>` of each top-level project.

## License

Apache Taverna is distributed under the
[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0)
