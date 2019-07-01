# APYBAC
An **A**rduino+**py**thon **B**lood **A**lcohol **C**ontent project. It's a fun project where you can estimate how drunk you are! It doesn't provide a metric with units, as the measurements must be calibrated. This process is left as an exercise for the reader. 

## Description of Setup
### Arduino
We equipped an Arduino with a [MQ-3](https://www.sparkfun.com/datasheets/Sensors/MQ-3.pdf) sensor. The MQ-3 is a cheap alcohol gas sensor with an analog readout. The C code for this setup is lost, but we do a simple readout from one of the analog pins where the sensor is attached. We print the output to the serial console. 

### PC
A jupyter notebook connects to the Arduino over USB and asynchronously reads the output while updating a figure over the current levels of alcohol. 


### Requirements
`pip install -r requirements.txt`

## How to use
1. Start jupyter lab: `jupyter lab`
2. Attach USB to a laptop.
3. Wait for the sensor to warm up, around 1-2 minutes. 
4. Breathe slowly with the mouth open wide, onto the sensor. 
5. Record the peak value. 
