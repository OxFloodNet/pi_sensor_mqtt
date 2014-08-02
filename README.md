#pi_sensor_mqtt

*Not currently developed: NodeRed being used instead.*

Lightweight gateway python code to read sensor data from serial wireless sensors and publish to an MQTT broker.


## Requirements

 * Python 3.2
 * virtualenv & virtualenvwrapper (http://virtualenvwrapper.readthedocs.org/en/latest/)

## Setup
    
    git clone https://github.com/sushack/pi_sensor_mqtt.git
    cd pi_sensor_mqtt
    source /usr/bin/virtualenvwrapper.sh
    workon pi_sensor_mqtt
    pip install -r requirements.txt
    
Copy config.example.yml to config.yml and add details for your gateway uuid, serial port, sensors, MQTT broker, etc.

Plug in the serial receiver and make sure you have read permissions on the device:

    sudo chmod a+r /dev/ttyACM0

There are better ways of doing some of the steps above, but configuring those is left as an exercise for the reader.

## Run

    ./sensor_mqtt.py
    
## License

This code is released as Open Source under the MIT license. See LICENSE.md for details.
