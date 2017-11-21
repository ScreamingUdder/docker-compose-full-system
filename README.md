# Full-System docker-compose Script

A docker-compose script for as many of our system services as possible.
Intended to be used for integration testing and functional testing of individual components. The Kafka broker is accessible at `localhost:9092`.

Included:
- NeXus file producer (https://github.com/ScreamingUdder/isis_nexus_streamer_for_mantid)
- Kafka-Manager (https://github.com/yahoo/kafka-manager)
- Kafka broker (https://hub.docker.com/r/wurstmeister/kafka/)
- Zookeeper (https://hub.docker.com/_/zookeeper/)
- EPICS IOC for a simulated ESS chopper (uses LeWIS https://github.com/DMSC-Instrument-Data/lewis)

Currently missing:
- Other EPICS IOCs (https://github.com/ScreamingUdder/simulated-iocs-docker)
- EPICS to Kafka forwarder (https://github.com/ess-dmsc/forward-epics-to-kafka)
- NeXus file writer (https://github.com/ess-dmsc/kafka-to-nexus)
- Make custom Kafka broker image with graphite reporter (https://github.com/damienclaveau/kafka-graphite)
- Graphite storage for metrics
- Grafana dashboard to monitor Kafka
- Mantid (https://github.com/mantidproject/mantid)
- NICOS?
