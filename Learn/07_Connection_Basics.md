## Connection Basics

1. When two devices are connected, they communicate periodically.

1. Master sends atleast one packet every connection interval(even if there  is no data to send so as to keep connection alive)

1. Slave - A slave can send a packet as a response to the packet of the master after 150us. (Refer the image BLE connection)

1. Connection interval varies from 7.5ms to 4000ms

1. Data payload is up 244 bytes/packet

1. Multiple packets can be sent in one connection interval

1. Slave devices can use slave latency enables them to skip N connection intervals if there is no data to transmit