##### WARNING

This project has been discontinued and it is not longer maintained since Neo4j does not rely on this wrapper anylonger.

Please consider procrun from Apache Foundation as a replacemet, more info availbale at [their website](http://commons.apache.org/proper/commons-daemon/procrun.html).

----------

This is a custom, slimmed down implementation of a service wrapper for Neo4j.

The starting point and bulk of the implementation is the 3.2.7 version of the JNA
library at

http://java.net/projects/jna

Its sources and latest version are not available through maven however so they were imported from
the source repository and trimmed down to the Windows needed parts only.

The basic use case is starting and stopping the Neo4j REST Server from the distribution
directory. Installation, removal and quering of the service is achieved via batch scripts,
leaving only the interaction with the windows ServiceManager to Java code.
