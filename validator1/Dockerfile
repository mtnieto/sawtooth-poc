FROM hyperledger/sawtooth-validator:latest

ADD validator.toml /etc/sawtooth/validator.toml

CMD  ["sawtooth-validator", "-vv", "--endpoint", "tcp://validator:8800", "--bind", "component:tcp://eth0:4004", "--bind", "network:tcp://eth0:8800"] 
     