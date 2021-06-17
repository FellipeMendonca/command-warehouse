# Metadata for a given topic

## If you want to see metadata for just one topic, specify it using (-t) parameter:
kafkacat -L -b broker -t topic
kafkacat -L -b broker -t topic -c qtd

<!-- -X  prop=val-->

kafkacat -b 127.0.0.1:9094 -t py-kafka-skin-json -L -C -o beginning

kafkacat -b 127.0.0.1:9094 -t py-kafka-skin-json -X socket.timeout.ms=50 -X session.timeout.ms=100 -C -o beginning

kafkacat -d broker,protocol,metadata,topic -b 127.0.0.1:9094 -t py-kafka-skin-json -C

kafkacat -b 127.0.0.1:9094 -L

kafkacat -b 127.0.0.1:9094 -t py-kafka-skin-json -P

kafkacat -C -b 127.0.0.1:9094 -t py-kafka-skin-json -o beginning