## Other Options for Power Savings

1. Voltage Scaling: Tradeoff between speed and consumption

BG22 Supports 3 voltage settings
    
- 1.1V
- 1.0V
- 0.9V

    1. EM0/1 High Performance: 1.1V upto 80MHz
    1. EM0/1 Normal Performance: 1.0V upto 40MHz
    1. EM0/1 Low performance: 0.9V upto 24MHz
    1. EM2/3: 0.9V upto 32KHz

- Crystal Settings:

    - BLE spec requires a clock with atleast 500ppm accuracy.
    - BG22 has a LFRCO(Low Freq RC Oscillator) which can provide this accuracy when precious mode is used.
    - More current consumption if continous calibration is enabled
    - Compared to external oscillator the accuracy is lower.
    - Advantage: If no external oscillator is used HW size and cost is low.

- PA Mode (Power Amplifier)

    - It is not enough to just set the TX power level, the PA mode has to be set accordingly.

    - With high power modes, the consumption will be bigger, even when TX is set to 0dBm

    - 6dBm cant be used in low power mode

    - At 0dBm with high power PA needs 44uA with low power PA only 38uA

- The ARM debug unit can be shutdown in EM2. As default it is enabled in example loades after it is switched off, it can only be enabled again via simplicity commander (device recovery)

- Switch Off VCOM/ Debug log

    - It is general hint to disable the usage of VCOM port and any debug prints in order to save energy
    - If it is a connectable device, you can change the advertising interval if a scan request receieved. so the connection process can be finished faster.
