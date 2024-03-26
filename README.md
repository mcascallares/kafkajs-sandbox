# Kafkajs Sandbox

This repo is a getting started project to easily get a producer app running using 
[KafkaJS](https://kafka.js.org/versions) client

## Requirements

- nvm
- confluent CLI

## Install and configure nodejs using nvm

```
nvm install v20.11.1
```

```
nvm use v20.11.1
```

## Install dependencies

```
npm install
```

## Launch kafka brokers for development

```
confluent local kafka start --brokers 1
```

## Execute producer app

```
node producer.js
```


## Consume messages from topic-test using Kafka CLIs

```
kafka-console-consumer --bootstrap-server localhost:9092 --topic topic-test --from-beginning
```
