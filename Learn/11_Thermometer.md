## A Thermometer Application

1. Let us see another example, this is another typical usage of a BLE device, it implements one service, which provides temperature measurement values at every second

1. Advertising parameter:

    - TX powers is 0dBm;
    - Advt interval: 500msec
    - Advt on all three channel
    - Advt payload: UUID of thermometer service, device name: XG22
    - Connectable and scannable
    - Average current consumption when advertising 17uA

1. Connection Parameter:

    - Connection interval: 100msec
    - Payload: Min.5bytes of data is sent every sec
    - Tx Power: 0dBm
    - With slave latency set to 0, average consumption: 19.5uA
    - With slave latency set to 5, average consumption is 12uA