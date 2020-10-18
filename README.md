# docker-mosquitto-mqtt

## Up mosquitto service

`$ docker-compose up -d`

`$ docker exec -it mosquitto sh`

## Test example mosquitto sub-pub

`$ mosquitto_passwd -c /mosquitto/config/pwfile username`

`$ mosquitto_sub -h localhost -u username -P password -v -t 'test-mosquitto'`

`$ mosquitto_pub -h localhost -u username -P password 1234 -t 'test-mosquitto' -m 'test message'`
