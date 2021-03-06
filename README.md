# Tsl2591-Light-sensor
The Tsl2591 Luminosity sensor measures visible+IR+full spectrum light values

## Schematic Design
This is my breadboard schematic design as follows:
![Schematic](https://user-images.githubusercontent.com/55503392/74797626-869afe80-5299-11ea-9aa0-502505d1a43c.png)

## PCB Design
This is my PCB design for the project
![pcb design](https://user-images.githubusercontent.com/55503392/74798727-82241500-529c-11ea-9e4c-b29585048298.png)

## PCB layout
This is my PCB connected to the sensor along with the Neopixel ring
![pcb_wiring](https://user-images.githubusercontent.com/55503392/74799922-ec8a8480-529f-11ea-9064-0470e414cc29.png)

## Breadboard Layout
![BreadBoard wiring](https://user-images.githubusercontent.com/55503392/74857282-758dd400-5311-11ea-841c-81878ac72c5b.png)

## Connection descriptions
The 3.3v pin from the Pi connects to the Vin of the sensor and provides it with power. Both the GND connections for the Pi and the sensor are connected together on the PCB. The Pi Synchronized clock pin connects to the sensor SCK pin. The Pi SDA pin is connected with the sensor SDA pin. Furthermore to connect the Neopixel ring I have to use a SN74AHCT125 3.3v to 5v level converter chip. The Pi's GPIO 18 pin is connected to the Pi's 1A pin. The pin 1Y from the chip connects to the Din pin of the ring to provide it the appropriate 5v data from the Pi. The GND of the power supply is connected to the one of the 74AHCT125 chip along with pin 10E. The power supply GND is also connected to the Pi and Neopixel GND. The power supply's 5v is connected to the converter chip's VCC along with the Neopixel 5v power input.
