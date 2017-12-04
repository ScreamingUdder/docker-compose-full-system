# Full-System docker-compose Script

A docker-compose script for as many of our system services as possible.
Intended to be used for integration testing and functional testing of individual components. The Kafka broker is accessible at `localhost:9092`.

Included:
- NeXus file producer (https://hub.docker.com/r/screamingudder/nexusproducer/)
- Kafka-Manager (https://hub.docker.com/r/sheepkiller/kafka-manager/)
- Kafka broker (https://hub.docker.com/r/wurstmeister/kafka/)
- Zookeeper (https://hub.docker.com/_/zookeeper/)
- EPICS IOC for a simulated ESS chopper (uses LeWIS https://github.com/DMSC-Instrument-Data/lewis)
- Event sum stream processor (https://hub.docker.com/r/screamingudder/event-sum-stream-processor/)
- Graylog server (https://hub.docker.com/swcc/docker-graylog2)
- NeXus file writer (https://github.com/ess-dmsc/kafka-to-nexus)

Currently missing:
- EPICS to Kafka forwarder (https://github.com/ess-dmsc/forward-epics-to-kafka)
- Custom Kafka broker image with graphite reporter (https://github.com/damienclaveau/kafka-graphite)
- Graphite storage for metrics
- Grafana dashboard to monitor Kafka

Possible other additions:
- Other EPICS IOCs (https://github.com/ScreamingUdder/simulated-iocs-docker)
- Mantid (https://github.com/mantidproject/mantid)
- NICOS
