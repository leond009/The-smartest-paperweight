# The-smartest-paperweight

Hi there! Im happy to present you the smartest paperweight ever!

As the name suggests, the project is a hockey puck sized thing(?) that you can interact with it. Essentially, it features many sensors to detect what is going on around it and reacts accordingly to each change (Specifically, to temperature, humidity, light and motion). This project is meant to be kept as a small companion on your desk and keep you company through its OLED screen and RBG led. The idea came to me after seeing the MESS i had in my desk and realizing that even inanimate object that don't really serve a purpose can also bee companions, and i took that idea to the next level.

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

PARTS LIST of the funding list
| [Esp32-S3-N16R8](https://www.electronicadiy.com/products/placa-de-desarrollo-wifi-bluetooth-esp32-s3-n16r8?variant=48511995019522) | Microcontroller of the project | 1 | $15.32 | $15.32 | [Electronica DIY](https://www.electronicadiy.com/products/placa-de-desarrollo-wifi-bluetooth-esp32-s3-n16r8?variant=48511995019522) |
| [Oled screen 1.3" SH1106 I2C](https://www.electronicadiy.com/products/pantalla-oled-1-3-sh1106?variant=43320054612226) | Screen to display the eyes of the PW | 1 | $11.26 | $11.26 | [Electronica DIY](https://www.electronicadiy.com/products/pantalla-oled-1-3-sh1106?variant=43320054612226) |

OTHER PARTS (that i already had lol)
| [TP4056](https://www.electronicadiy.com/products/modulo-de-carga-tp4056-con-proteccion) | Charging | 1 | $1.00 | $1.00 | [Electronica DIY](https://www.electronicadiy.com/products/modulo-de-carga-tp4056-con-proteccion) |
| [AMS1117](https://www.electronicadiy.com/products/convertidor-de-voltaje-5v-a-3-3v-ams1117?_pos=2&_sid=f3598c96b&_ss=r) | Power regulation| 1 | $0.50 | $0.50 | [Electronica DIY](https://www.electronicadiy.com/products/convertidor-de-voltaje-5v-a-3-3v-ams1117?_pos=2&_sid=f3598c96b&_ss=r) |
| [DHT111](https://www.electronicadiy.com/products/sensor-de-temperatura-y-humedad-dht11-ky-015?_pos=1&_sid=ee95e7ec1&_ss=r) | Temperature and Humidity sensor| 1 | $3.00 | $3.00 | [Electronica DIY](https://www.electronicadiy.com/products/sensor-de-temperatura-y-humedad-dht11-ky-015?_pos=1&_sid=ee95e7ec1&_ss=r) |
Resistors and minor extra components are not disclosed, everyone has one laying around haha
