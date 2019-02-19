chinadns + dnsmasq
==================

## About

- chinadns: Protect yourself against DNS poisoning in China.
- dnsmasq: A free software DNS forwarder and DHCP server for small networks

## Run

    docker run -d --name chinadns -p 53:53 -p 53:53/udp --restart=always vank3f3/chinadns

## Test

    # UDP
    dig @YOUIP www.google.com

    # TCP
    dig @YOUIP www.youtube.com +tcp

