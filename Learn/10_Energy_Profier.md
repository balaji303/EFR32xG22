## Energy Profiler

1. To measure the energy consumption checkout the tool called energy profiler. Checkout UG343 in Simplicity Studio.

## Low Energy Beacon:

1. The following config are required to be implemented for a low energy beacon:

    - Advertising interval 1 second
    - Advertise only one channel
    - Not scannable, not connectable
    - Advertising payload: just the device name "BG22" alone
    - Tx power: 0dBm
    - PA is set to low energy mode
    - The average current consumption is about ~4,5uA in this case.