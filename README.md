[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-v2.0%20adopted-ff69b4.svg)](CODE_OF_CONDUCT.md)

# Solace Distributed Tracing Demo

## Overview
This project contains the assets and applications needed to run an end to end distributed tracing demo. This repo contains the following:

* `docker-compose.yaml` containing the following:
  * Docker image of the Solace PubSub+ Event Broker
  * Docker image of the [OpenTelemetry Collector Contrib](https://github.com/open-telemetry/opentelemetry-collector-contrib) packaged with a Solace receiver modules
  * Docker Image for the Jaeger all in one
* `otel-collector-config.yaml` - configuration file needed for collector
* `solace_config_keys.env` - env variables for configuring the solace broker
* `.env `- contains env variables for the docker compose file
* `src/solace-publisher.jar` - Solace JMS application for publishing of messages
* `src/solace-queue-receiver.jar` - JMS application for receiving messages from a JMS Queue
* `src/opentelemetry-javaagent-all-1.19.0.jar` - [OpenTelemetry Java Instrumentation](https://github.com/open-telemetry/opentelemetry-java-instrumentation) API to dynamically inject telemetry bytecode
* `src/solace-opentelemetry-jms-integration-1.0.0.jar` - [Solace PubSub+ OpenTelemetry Integration API for JMS](https://repo1.maven.org/maven2/com/solace/solace-opentelemetry-jms-integration/1.0.0/solace-opentelemetry-jms-integration-1.0.0.jar)
* `src/jms-auto-instrumentation-sampler-sources.jar` - Source code for the Solace jms application for publishing and receiving messages

## Getting started quickly
Follow the steps in this [codelab](https://codelabs.solace.dev/codelabs/dt-otel/index.html) for details

## Documentation
Details about the what why and how of this project. Either refer to external documentations or document in this repo

## Resources
This is not an officially supported Solace product.

For more information try these resources:
- Ask the [Solace Community](https://solace.community)
- The Solace Developer Portal website at: https://solace.dev


## Contributing
Contributions are encouraged! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.

## Authors
See the list of [contributors](https://github.com/solacecommunity/<github-repo>/graphs/contributors) who participated in this project.

## License
See the [LICENSE](LICENSE) file for details.
