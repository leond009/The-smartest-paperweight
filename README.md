# The-smartest-paperweight

Hi there! Im happy to present you the smartest paperweight ever!

The name is an oxymoron bc esseantialy the project is a mere distraction or fun toy, not necesarrily something that adds any valua. (Unless it is crucial for you to read the weather through the very precise metric of digital googly eyes).

Here is a thourough description of what each component does:

Sensors and Internal components that the user does not interact with:
~ It features the MPU6050 Gyroscope and accelerometer to detect movement of the project and have the reactive components react accordingly to the movement. It is also planned that in order to check information of the weather, humidity and temperatre, the user moves the paperweight with a certain gesture.
~ It features a Photoresistor paired with a 10kohm resistor to react to sorrounding light. I included this to make sure the paperweight didnt become to distrative at night and also possibly include it in weather reaction.
~ It fetures the DHT11 sensor to detect humidity and temperature. Because of this sensor it is very important that the case is not fully enclosed, otherwise the measurements become not onlz inaccurate but one of tha main purposes of the Paperweight (Ambient reaction) is rendered useless.
~ To power the whole project, I plan to use a 100mAh(This can eventually be changed to a battery with larger capacity) Lipo battery paired with the TP4056 to charge the battery.
~In order to prevent any damage caused by power fluctuations as some of the components are directly powered through the battery, i included the AMS1117 for power regulation.
~The whole system is controlled with an ESP32, eventually, through Bluetooth the user can change the color of the paperweight according to what the PW is sensing.

Components that the user interacts with:
~The project features and 1.13 inch OLED controlled with I2C to save up on GPIO pins. On the display two robot eyes are displayed and they react to the environment according to what the sensors are measuring. Moreover, using the gestures measured with the MPU6050, the user can check the power left on the battery
~The project also features an RBG led paired with 330 OHM resistors to change the color of the paperweight. (Nothe that this means that the enclosure MUST be translusent or transparent)
~Thanks to the TPU4056 the user can charge the battery using a simple microUSB cable.


Here are some pictures of the project!
![Fornt of the PCB](ThesmpwFRONT.png)
![Back of the PCB](ThesmpwBACK.png)
