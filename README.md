# EmbeddedMonitoringSystem
Tracks temperature and current draw data and logs this in persistent storage.

# Processor and Summary 
Using the ATtiny85, programmed using Arduino as ISP.

# Sensor circuits
Temperature measured using thermistor in a voltage divider circuit.
Voltage of fixed resistor is measured on ATtinys ADC pin.
Digital value is converted back to its original analogue voltage, this is used to figure out the resistance of the thermistor.
This resistance as well as datasheet parameters are input to the Steinhart equation to figure out temperature in Kelvin which is converted to degrees C.