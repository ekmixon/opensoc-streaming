# OpenSOC-Streaming

Extensible set of Storm topologies and topology attributes for streaming, enriching, indexing, and storing telemetry in Hadoop.


## Usage

mvn clean
mvn install

This will build all the projects at the same time

Navigate to OpenSOC-Topologies/target
Maven should build OpenSOC-Topologies-0.0.1-SNAPSHOT.jar

To run the Bro topology:
storm -jar /path/to/OpenSOC-Topologies-0.0.1-SNAPSHOT.jar ./storm jar com.opensoc.topologies.BroEnrichmentTestTopology

To run the Sourcefire topology:
storm -jar /path/to/OpenSOC-Topologies-0.0.1-SNAPSHOT.jar ./storm jar com.opensoc.topologies.SourcefireEnrichmentTestTopology

## Importing to Eclipse

I would recommend switching to a new workspace, but that is optional

In Eclipse perform the following actions:

File->Import->maven->existing maven project
Point to the checked out GIT repo