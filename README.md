# loadbalance_ML

Data science task
Non intrusive load monitoring or NILM involves analysing and disaggregating electricity usage
by appliances connected to a power supply. This allows power users to learn more about how
they use electricity. The aim of this task is to build a machine learning based algorithm that
automatically and accurately identifies what appliances are connected to the power supply.

Data Description :
Data is collected using a current(mA) sensor attached to the wire of the main power supply. In
the current simulation environment a total of 3 devices are connected to the power supply:
    ● 2 normal PC displays and
    ● 1 temperature sensor.
    
The PC display can be in 3 states: OFF, IDLE and ON.
The temperature sensor can be in 2 states: ON or OFF.


    ● test_data1536128609.98_screen1.csv contains the data when only the 1st PC display
    is connected to the power supply and other 2 devices are disconnected. It contains the
    current data from the PC display.
    ● test_data1536128871.84_screen2.csv contains the data when only the 2nd PC display
    is connected to the power supply and other 2 devices are disconnected. It contains the
    current data from the PC display.
    ● test_data1536129261.77_device253.csv contains the data when only the temperature
    sensor is connected to the power supply and other 2 devices are disconnected. It
    contains the current data from the temperature sensor.
    ● test_data1536129670.55_main.csv - contains the data when all 3 devices are
    connected to the power supply.
    
All csv files follow the format defined below:
    ● Timestamp
    ● Maximum current(mA) value detected within one second
    ● Effective current(mA) value detected within one second
    
Problem Statement
Provide a machine learning based program which:
● receives as an input file test_data1536129670.55_main.csv, and
● Produces as an output 1 (one) .csv file containing the state for each device.


