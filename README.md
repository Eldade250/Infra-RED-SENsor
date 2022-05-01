# TURN ON RED BY USING AN ACTIVE IR LED SENSOR
# ABSTRACT
turning ON an LED using IR sensor and ARDUINO UNO is a system that was created to reduce power consumption and to above power saving when sensors are used in this project. The sensor will control electricity supply by detecting the presence of in-room . Additionally, another function for this project is to control supply electricity. The objectives of this project are to reduce the waste of power to save the environment and save the cost of electric power for universities and taxpayers. If no appearance is detected, no output will go out and supply is still being turned off. ARDUINO UNO that will be used to connect hardware with LED and Active IR sensor electronic functions. For the time being come, this system can be applied in lecture rooms, office houses and like security on get, Bathroom and so on. 
 
# PROBLEM STATEMENT 
 
Nowadays excessive and uncontrolled use of electricity have become one of the sources of increasing large time. This is why there is an initiative in improving the existing wiring system to more systematic and user-friendly. Today’s switchgear switches are seen as the cause of user negligence resulting in an increase in electricity and unexpected events. Besides that, people start to find more easier or convenient solution in daily life. Electronic technology is popular nowadays because it is convenient, easier to construct and save cost. Then, they also can access to this system anytime. Moreover, this system is easy to build and configure.

# DISCRIPTION OF THE CIRCUIT

# ARDUINO UNO
 
Arduino Uno is a microcontroller board based on the ATmega328P (datasheet). It has 14 digital input/output pins (of which 6 can be used as PWM outputs), 6 analog inputs, a 16 MHz quartz crystal, a USB connection, 
A power jack, an ICSP header and a reset button. It contains everything needed to support the microcontroller; simply connect it to a computer with a USB cable or power it with an AC-to-DC adapter or battery to get started. You can tinker with your UNO without warring too much about doing something wrong, worst-case scenario you can replace the chip for a few dollars and start over again. 
"Uno" means one in Italian and was chosen to mark the release of Arduino Software (IDE) 1.0. The Uno board and version 1.0 of Arduino Software (IDE) were the reference versions of Arduino, now evolved to newer releases. The Uno board is the first in a series of USB Arduino boards, and the reference model for the Arduino platform
 
# IR SENSOR MODULE
 
This Infrared obstacle/object detection sensor is super easy to use. It comes with on board potentiometer to adjust the sensitivity. The output is digital signal so it is easy to interface with any microcontroller such as Arduino/Genuino UNO, Mega, Zero, 101, even the Raspberry Pi or Raspberry Pi Zero. And of course it is also compatible with all other controller boards out there including CIKU, CT-UNO, CT-ARM, etc. This Infrared sensor offers simple, user friendly and fast obstacle detection via infrared reflection, it is non contact detection. As it is based on light reflection, the detection do vary with different surface. And any infrared source might also interfere the detection 
It comes in a pair of Infrared emitter and receiver at the front of module, whenever there is object blocking the infrared source, it reflects the infrared and the receiver get it and the signal go through a comparator circuit on board. And depending on the threshold that being adjusted, it will output logic LOW at output pin and the green LED will light up to indicate the detection. Turning the on board potentiometer clock wise will increase the sensitivity and further increase the detection range. Compatible with 5V or 3.3V power input. 
# LIGHT EMITTING DIODE (LED) 

Light-emitting diode (LED) is a semiconductor device that emits light when an electric current is passed through it. Light is produced when the particles that carry the current (known as electrons and holes) combine together within the semiconductor material. 
Since light is generated within the solid semiconductor material, LEDs are described as solid-state devices. The term solid-state lighting, which also encompasses organic LEDs (OLEDs), distinguishes this lighting technology from other sources that use heated filaments (incandescent and tungsten halogen lamps) or gas discharge (fluorescent lamps). 
# WIRE CONNECTION
It is used to connect the components used in circuit.
 WORKING PRINCIPLE
 My project is to design of turning ON an LED using active IR sensor it has important, first is an infrared sensor is an electronic instrument that is used to sense certain characteristics of its surroundings. It does this by either emitting or detecting infrared radiation. when there is obstact object.
 
It has response time faster than thermocouple. It provides good stability over time. No corrosion or oxidation can affect the accuracy of infrared sensor
 

The emitter is an IR LED and the detector is an IR photodiode. The IR photodiode is sensitive to the IR light emitted by an IR LED. The photo-diode's resistance and output voltage change in proportion to the IR light received. The IR sensor is controlled under instruction of Arduino source code to turning LED  which can use high power and low power with good response and efficiency by using low supply.

# BLOCK DIAGRAM OF THE CIRCUIT
![image](https://user-images.githubusercontent.com/104734132/166161232-4ea9f8f8-6e7c-47a3-82fc-dc8aff2764bb.png)

# SOURCE CODE OF ARDUINO UNO

int IR=8;

int led=13;

void setup() {

pinMode (13, OUTPUT);

pinMode(8,INPUT);

Serial.begin(9600);

}

void loop()

{IR=digitalRead(8);

  if (digitalRead(8)== LOW)
  
  {
  
    digitalWrite(13,HIGH);
    
 
 
  }
  
  else 
  
  {
    
    digitalWrite(13,LOW);
    
  }
  
}


CIRCUIT DIAGRAM IN PROTEUS
![image](https://user-images.githubusercontent.com/104734132/166161189-afae522f-70cc-4fc2-ab7e-1d13c0aa8b30.png)


CIRCUIT DIAGRAM IN FRITZING
 ![image](https://user-images.githubusercontent.com/104734132/166161198-8ef8b975-6370-40ba-bfaf-c872e825fe57.png)

NAMES;NDAYAMBAJE Eldade
              SHYIRAMUNDA Sylvain 
 
