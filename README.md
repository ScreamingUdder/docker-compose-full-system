# Full-System docker-compose Script

A docker-compose script for as many of our system services as possible.
Intended to be used for integration testing and functional testing of individual components. The Kafka broker is accessible at `localhost:9092`.

Included:
- NeXus file producer (https://hub.docker.com/r/screamingudder/nexusproducer/)
- Kafka-Manager (https://hub.docker.com/r/sheepkiller/kafka-manager/)
- Kafka broker (https://hub.docker.com/r/wurstmeister/kafka/)
- Zookeeper (https://hub.docker.com/_/zookeeper/)

Currently missing:
- EPICS IOC for a simulated device (will use https://github.com/DMSC-Instrument-Data/lewis)
- EPICS to Kafka forwarder (https://github.com/ess-dmsc/forward-epics-to-kafka)
- NeXus file writer (https://github.com/ess-dmsc/kafka-to-nexus)
- Make custom Kafka broker image with graphite reporter (https://github.com/damienclaveau/kafka-graphite)
- Graphite storage for metrics
- Grafana dashboard to monitor Kafka
- Mantid (https://github.com/mantidproject/mantid)
- NICOS?
