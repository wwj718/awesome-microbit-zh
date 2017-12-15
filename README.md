# micro:bit资源大全中文版  [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[![micro:bit logo](https://i.imgur.com/rYLbkBh.jpg)](https://www.microbit.org)

micro:bit 是一款由英国广播电视公司（BBC）推出的为青少年编程教育设计的微型电脑开发板, 集成了低功耗蓝牙，加速度计，磁力计，三个按钮，5 x 5 LED点阵以及GPIO。

本列表翻译自[awesome-microbit](https://github.com/carlosperate/awesome-microbit) ，是由 [carlosperate](https://github.com/carlosperate) 发起并维护的microbit资源列表。

Awesome-XXX 是GitHub上知名的一组项目，其主页：[Awesome 清单](https://github.com/sindresorhus/awesome/blob/master/awesome.md)

欢迎大家提交有趣的项目 :)

## 目录

- [编程](#programming)
	- [Visual](#visual)
	- [Python](#python)
	- [JavaScript / MakeCode](#javascript-and-makecode)
	- [C/C++](#cc)
	- [其他 micro:bit 程序语言](#other-microbit-languages)
	- [其他交互语言](#other-interaction-languages)
- [编程工具](#programming-tools)
- [移动应用](#mobile-apps)
- [ChromeOS应用](#chromeos-apps)
- [Interface Chip](#interface-chip)
- [硬件](#hardware)
- [CAD 与 3D打印](#cad--3d-printing)
- [项目](#projects)
- [文章](#articles)
- [视频](#videos)
- [书籍](#books)
- [教学资源](#teaching-resources)
- [社区](#community)
- [杂项](#miscellaneous)


## 编程

### 图形化编程

- [MakeCode](https://makecode.microbit.org) - 提供一个基于浏览器的模拟器和积木编程环境，堆叠好的积木块最终将生成JavaScript (TypeScript)代码 (之前以PXT为人所知).
- [Microsoft Blocks](https://www.microbit.co.uk/app/#create:xczaux) - 积木风格的交互界面. 该项目已不再开发，推荐大家使用 MakeCode 替代它.
- [Code Kingdoms](https://www.microbit.co.uk/app/#create:tomwku) - 基于图形界面的编程工具，帮助用户从拖曳式编程到文本编程(JavaScript)的过渡.
- [Scratch for BBC micro:bit](http://www.picaxe.com/BBC-microbit) - 将micro:bit用作Scratch/S2Bot的蓝牙游戏控制器(蓝牙控制手柄) (需要特殊的BLED112蓝牙适配器).
- [Open Roberta Lab](http://lab.open-roberta.org) - 为机器人编程设计的积木时编程环境, 通过将堆叠好的积木生成MicroPython代码来支持microbit.
- [ScratchX micro:bit extension](https://llk.github.io/microbit-extension/) - 让你使用Scratch编程积木块控制microbit.

### Python

- [microbit-micropython](http://microbit-micropython.readthedocs.io) - 移植于MicroPython, MicroPython是Python3的一种实现，用于微控制器和受限环境

##### MicroPython 编辑器

- [microbit.org Python editor](https://python.microbit.org) - 来自micro:bit官方的Python在线编辑器
- [microbit.co.uk Python editor](http://microbit.co.uk/app/#create:xyelfe) - 最早的Python在编辑器, 包含了旧版的 MicroPython.
- [Mu](http://codewith.mu) - MicroPython与micro:bit的离线编辑器
- [create.withcode.uk](https://create.withcode.uk) - python在线编辑器，带有模拟器 ([instructions](http://community.computingatschool.org.uk/resources/4479)).
- [Atom microbit-micropython](https://github.com/wendlers/atom-microbit-micropython) - Atom 编辑器的micro:bit MicroPython扩展包（插件）.
- [Thonny micro:bit](https://bitbucket.org/KauriRaba/thonny-microbit/wiki/installation-guide) -  [Thonny](http://thonny.org)插件, Thonny是面向初学者的pythonIDE
- [JetBrains IDEA/PyCharm IDE plugin](https://plugins.jetbrains.com/plugin/9777-micropython-support) - 使IntelliJ IDEA 和 PyCharm支持MicroPython设备的插件.

##### MicroPython 库

- [Servo](https://github.com/microbit-playground/microbit-servo-class) - microbit中通过产生PWM波（脉宽调制）来控制舵机的简单类库。
- [PCA9685](https://github.com/gingemonster/PCA9685-Python-Microbit) - 通过IIC总线来控制PCA9685（一个16通道 12bit位分辨率的PWM/舵机伺服器芯片）的简单类库。
- [MAX7219 7-segment](https://github.com/microbit-playground/matrix7seg) - 通过SPI总线驱动的用于控制七段数码管的MAX7219芯片的相关MicroPython模块。
- [MAX7219 matrix](https://github.com/titimoby/microbit4all/blob/master/libraries/matrix7219.py) - 通过SPI总线驱动的用于控制8×8发光二极管点阵的MAX7219芯片的相关MicroPython模块。
- [SSD1306](https://github.com/fizban99/microbit_ssd1306) - microbit中通过I2C总线用于控制SSD1306（128*64分辨率）OLED屏幕的MicroPython库。
- [SSD1306 7seg](https://github.com/fizban99/microbit_ssd1306_7seg) - 用于使用SSD1306 OLED屏幕去模拟七段数码管的MicroPython库。 
- [SSD1306 SPI](https://github.com/fizban99/microbit_ssd1306spi) - microbit中通过SPI总线去控制SSD1306（128×64分辨率）OLED屏幕的MicroPython库。
- [HT16K33](https://bitbucket.org/thesheep/microbit-ht16k33) - 用于多种配置（16x8,8x8或8x8x2）的HT16K33 LED点阵驱动器的MicroPython库。
- [HC-SR04](https://github.com/fizban99/microbit_hcsr04) - 通过SPI总线来读取从 HC-SR04 超声波传感器获取的距离的基本MicroPython库。
- [US-100](https://github.com/fizban99/microbit_us100) - 通过UART从US-100 超声波传感器读取距离的基本MicroPython库。
- [KY038](https://github.com/fizban99/microbit_ky038) - 校准和使用 KY038 声音传感器的MicroPython库，包含拍手计数器功能。
- [Nokia 5110 PCD8544 LCD](https://github.com/matneee/microbit-nokia5110-PCD8544-lcd) - Micro:bit中用于控制Nokia 5110 LCD显示屏的MicroPython控制器。
- [MPL115A1](https://github.com/hackscribble/microbit-MPL115A1-barometer) - 通过SPI总线读取NXP MPL115A1 压力传感器的压力以及温度数值的MicroPython类
- [24LCxxx EEPROM](https://github.com/matneee/microbit-I2C-EEPROM-24LCxxx-Read-Write) - 用于读取和写入I2C EEPROM（24LCXXX型号）的Micro:bit函数的例子
- [ULN2003](https://github.com/IDWizard/uln2003) - 通过ULN2003达林顿晶体管阵列来驱动步进电机的Micropython代码。

##### Python 库

- [MicroPeri](https://github.com/c0d3st0rm/microperi) - 使用micro:bit MicroPython API在电脑上运行Python程序以及作为外围设备或传感器连接micro:bit.
- [microbit_stub](https://github.com/casnortheast/microbit_stub) - 模拟micro:bit MicroPython API的Python库
- [bluezero](https://github.com/ukBaz/python-bluezero) - 与蓝牙设备交互的Python包，里边带有micro:bit的例子
- [bitio](https://github.com/whaleygeek/bitio) - BBC micro:bit Python I/O 库. 允许你在 PC/Mac/Linux/Raspberry Pi上边直接跑Python代码并直接与 micro:bit交互（支持输入、输出）.如果你想把micro:bit作为外设与你既有的系统交互，这个库十分值得一试！

##### Python 编程工具

- [uFlash](https://github.com/ntoll/uflash/) - 用于往 micro:bit 中烧录Python脚本和 MicroPython 运行时的工具. （支持将python代码转为hex格式以及逆向操作）
- [MicroFs](https://github.com/ntoll/microfs) - 一个简单的命令行工具/模块,用于与micro:bit中的受限文件系统(由MicroPython提供)交互.
- [Jupyter kernel for the micro:bit](https://github.com/takluyver/ubit_kernel) - 允许你在Jupyter中使MicroPython代码直接运行在micro:bit上

### JavaScript 和 MakeCode

- [MakeCode](https://makecode.microbit.org) - 提供一个基于浏览器的模拟器和积木编程环境，堆叠好的积木块最终将生成JavaScript (TypeScript)代码 (之前以PXT为人所知).
- [Espruino JavaScript](http://www.espruino.com/MicroBit) - 用于微处理器的JavaScript引擎，它也提供一个同时支持文本和及木化编程的浏览器编程环境.
- [Code Kingdoms](https://www.microbit.co.uk/app/#create:tomwku) - 基于图形界面的编程工具，帮助用户从拖曳式编程到文本编程(JavaScript)的过渡.

##### MakeCode 库(pxt驱动)

- [Neopixel](https://github.com/Microsoft/pxt-neopixel) - Neo-Pixel(Neo-Pixel是一种流行的全彩led灯(每个led独立编址)，效果绚丽)的pxt驱动.
- [Filesystem](https://github.com/Microsoft/pxt-filesystem) - 文件系统的pxt驱动(测试版).
- [MAX6675](https://github.com/Microsoft/pxt-max6675) - MAX6675 pxt驱动.
- [Bluetooth MAX6675](https://github.com/Microsoft/pxt-bluetooth-max6675) -  MAX6675温度探头的蓝牙服务.
- [Sonar](https://github.com/Microsoft/pxt-sonar) -  超声波传感器的pxt驱动.
- [Bluetooth Temperature Sensor](https://github.com/Microsoft/pxt-bluetooth-temperature-sensor) - 温度传感器的蓝牙驱动.
- [MIDI](https://github.com/Microsoft/pxt-midi) - MIDI(乐器数字接口,为电子乐器等演奏设备定义各种音符或弹奏码) pxt驱动（测试版）.
- [Bluetooth MIDI](https://github.com/Microsoft/pxt-bluetooth-midi) - 蓝牙MIDI pxt驱动（测试版）.
- [BlueDot](https://github.com/Microsoft/pxt-bluedot) -  支持BlueDot app的PXT库(测试版).
- [GY521](https://github.com/PaulDFoster/pxt-microbit-GY521) -  为 Microbit 驱动 MPU-6050 (GY-521)（MPU6050是一种非常流行的空间运动传感器芯片，可以获取器件当前的三个加速度分量和三个旋转角速度）提供支持的PXT驱动.
- [UCL Junkrobot](https://github.com/chevyng/pxt-ucl-junkrobot) - 使用 28BYJ-48 步进电机 和 HC-SR04 超声波传感器控制的Junk机器人.
- [BitBot](https://github.com/srs/pxt-bitbot) - BitBot(使用microbit控制的一款小车)的pxt驱动.
- [gamer:bit](https://github.com/sparkfun/pxt-gamer-bit) - SparkFun gamer:bit扩展板(microbit驱动的游戏手柄)的pxt驱动.
- [moto:bit](https://github.com/sparkfun/pxt-moto-bit) -  SparkFun weather:bit扩展板(给你一个全功能的气象站)的pxt驱动.
- [weather:bit](https://github.com/sparkfun/pxt-weather-bit) - SparkFun weather:bit扩展板的pxt驱动.
- [SSD1306](https://github.com/Tinkertanker/pxt-ssd1306-microbit) - SSD1306 OLED 屏幕的pxt驱动, 基于Adafruit Arduino库.
- [mi:node](https://github.com/minodekit/pxt-minode) - Mi:node 套件(由element14提供的micro:bit IoT 起步套件) PXT驱动.
- [Kitronik Servo Lite](https://github.com/KitronikLtd/pxt-kitronik-servo-lite) - Kitronik Servo:Lite(驱动伺服电机) 扩展板的pxt驱动.
- [Kitronik I2C 16 Servo](https://github.com/KitronikLtd/pxt-kitronik-I2C-16-servo) - Kitronik I2C 16 Servo扩展板(驱动多达16个伺服电机)的pxt驱动.
- [Kitronik motor driver](https://github.com/KitronikLtd/pxt-kitronik-motor-driver) - Kitronik micro:bit电机驱动扩展板.
- [Lego Power Functions](https://github.com/philipphenkel/pxt-powerfunctions) - 使用micro:bit远程控制 LEGO® Power Functions电机的pxt扩展.
- [KY-040](https://github.com/Tinkertanker/pxt-ky040-microbit) - KY-040 旋钮编码器的pxt驱动.
- [Invent robot](https://github.com/techcampuk/pxt-invent) - Invent 机器人的pxt驱动.
- [Robotbit](https://github.com/KittenBot/pxt-robotbit) - KittenBot Robotbit的pxt驱动.
- [ubirch NB-IoT](https://github.com/ubirch/pxt-ubirch) - 发送加密数据到ubirch后端的pxt驱动（依赖BC95 NB-IoT 模组，它是一款高性能、低功耗的NB-IoT无线通信模块）.
- [CCS811](https://github.com/ADataDate/pxt-airQuality) - CCS811空气质量传感器模块(可提供等效二氧化碳（eCO2）等级或总挥发性有机化合物（TVOC）指标)的pxt驱动.
- [DS1307](https://github.com/Tinkertanker/pxt-ds1307-microbit) - 使用DS1307实时时钟(提供秒、分钟、小时、日、月、星期及年计时，带闰年补偿，有效期至2100年) (测试版)的pxt模块.
- [HT16K33](https://github.com/Tinkertanker/pxt-ht16k33-alnum4) - HT16K33 数字显示屏的pxt驱动 (测试版).
- [HoneyBit](https://github.com/HoneycombKits/pxt-HoneyBit) - Honeycomb 套件的pxt扩展.

##### Node.js库

- [node-bbc-microbit](https://github.com/sandeepmistry/node-bbc-microbit) - 使用蓝牙在Node.js中控制micro:bit 
- [node-bbc-microbit-io](https://github.com/sandeepmistry/node-bbc-microbit-io) - Johnny-Five (JavaScript机器人和IoT 编程平台) micro:bit IO 插件.

##### JavaScript前端库

- [microBit.js](https://github.com/antefact/microBit.js) - 一个前端库，使用web bluetooth AP来与micro:bit交互.

##### JavaScript编程工具

- [PXT Command Line Tool](https://makecode.com/cli) - 在命令行中使用MakeCode JavaScript为micro:bit编程。你也可以运行一个本地版本的MakeCode在线编辑器


### C/C++

- [C/C++ runtime](https://lancaster-university.github.io/microbit-docs/) - Guidance on how to start using the runtime in C/C++ including full documentation of the APIs, drivers, and types that make up the micro:bit runtime. Bluetooth documentation includes a link to the original `*.hex` file that ships on the micro:bit devices.
- [Arduino nRF5](https://github.com/sandeepmistry/arduino-nRF5/) - Arduino Core for Nordic Semiconductor nRF5 based boards, including the micro:bit.

##### C/C++编辑器

- [Micro:Pi](https://github.com/Bottersnike/Micro-Pi) - C/C++ editor for the micro:bit with serial monitor and deploy functionality. Written in Python with an installer (ATM Linux only, but could be manually installed in any OS) that includes all dependencies.

##### C/C++库

- [OneWire](https://github.com/adamboardman/microbit-onewire) - BBC micro:bit OneWire Library, based upon Erik Olieman's mbed DS1820 lib.
- [neopixel](https://github.com/elmorg/uBit_neopixel) - Library for using neopixels with the BBC micro:bit.
- [microbit Screen](https://github.com/ht-deko/microbit_Screen) - Arduino LED Screen library for micro:bit.
- [Adafruit Arduino MicroBit library](https://github.com/adafruit/Adafruit_Microbit) - Wrapper code and examples for using micro:bit with Arduino IDE.

### 其他 micro:bit 程序语言

- [Touch Develop](https://www.microbit.co.uk/create-code#touchdevelopEditor) - Flexible, text-based programming language with an interactive visual component.
- [Rust on BBC micro:bit](https://github.com/SimonSapin/rust-on-bbc-microbit) - Article describing the experience and steps of compiling Rust code for the micro:bit with and without interaction with the runtime DAL.
- [Forth](https://wiki.forth-ev.de/doku.php/en:projects:microbit:start) - Forth, a stack-based language, for the BBC micro:bit.
- [Pascal](http://wiki.freepascal.org/micro:bit) - Free Pascal compiler that can target the ARM embedded platform, including the micro:bit.
- [Ada](https://github.com/AdaCore/Ada_Drivers_Library/tree/master/examples/MicroBit) - Instruction on how to setup the Ada development environment for the micro:bit.

### 其他交互语言

- [Kodu Controller](http://www.kodugamelab.com/bbc-microbit/) - Enables interacting with the microbit from Kodu Game Lab.
- [Simulink Coder Support Package](http://uk.mathworks.com/matlabcentral/fileexchange/60273-simulink-coder-support-package-for-bbc-micro-bit-board) - Package that enables you to create Simulink models and automatically generate and deploy code on the micro:bit.
- [microbit for Dyalog APL on the Pi](https://github.com/APLPi/microbit) - Tools for using the micro:bit (via MicroPython serial connection) with the Dyalog APL programming language on the Raspberry Pi.
- [Gobot](https://gobot.io/documentation/platforms/microbit/) - Framework for the Go programming language to program devices in the real world. It can now the micro:bit via Bluetooth LE.
- [Microbit Unity](https://github.com/bLiGM/Microbit-Unity) - Unity scripts to allow the BBC Microbit to be used as a Unity Controller.
- [Haxe node BBC micro:bit](https://github.com/MatthijsKamstra/hx-node-bbc-microbit) - Control a BBC micro:bit from Node.js using BLE and the Haxe programming language.
- [App Inventor + IoT](http://iot.appinventor.mit.edu/#/microbit/microbitintro) - Control a micro:bit via Bluetooth with App Inventor, a visual programming environment for Android applications.
- [BlockyTalkyBLE](http://www.playfulcomputation.group/blockytalkyble.html) - MakeCode and App Inventor extension that makes it easy to connect AppInventor mobile phone apps with the BBC micro:bit wirelessly over Bluetooth.
- [DroidScript - MicroBit Plugin](https://play.google.com/store/apps/details?id=org.droidscript.microbit) - Allows you you to control the BBC micro:bit remotely from your own DroidScript apps (Android apps written in JavaScript).
- [CBMicroBit](https://github.com/Louismac/CBMicroBit) - CoreBluetooth wrapper in C++ that connects a micro:bit to a computer running OSX using BLE and outputs over OSC (can be used standalone, or as a C++ or Objective C library).


## 编程工具

- [Vagrant C/C++ Development Environment](https://github.com/carlosperate/microbit-dev-env) - Creates a virtual machine with all the toolchain required to compile and flash C/C++ and MakeCode programs to the micro:bit (including  MicroPython).
- [micro:bit uploader](https://www.touchdevelop.com/microbituploader) - Windows application that monitors your Downloads folder and flashes any new programs to the micro:bit.


## 移动应用

- [Official Android App](https://play.google.com/store/apps/details?id=com.samsung.microbit) ([Source Code](https://github.com/Samsung/microbit)) - Pair, program and flash programs to the micro:bit via Bluetooth.
- [Official iOS App](https://itunes.apple.com/gb/app/micro-bit/id1092687276) - Pair, program and flash programs to the micro:bit via Bluetooth.
- [micro:bit Blue](https://play.google.com/store/apps/details?id=com.bluetooth.mwoolley.microbitbledemo) ([Source Code](https://github.com/microbit-foundation/microbit-blue)) - Android app that contains a series demos for interacting with the micro:bit using Bluetooth.
- [Bitty Software Apps](http://www.bittysoftware.com/apps.html) - Diverse collection of Android and iOS apps, going from data logging to audio pranks, you'll certainly find something of interest. 
- [Insight Mr Bit](http://www.insightresources.co.uk/microbit/page63.html) ([iOS](https://itunes.apple.com/gb/app/insight-mr-bit/id1175915875)) - Create simple programs in plain English to control the BBC micro:bit to do lots of useful things.
- [Micro:bit Xamarin](https://play.google.com/store/apps/details?id=com.sumitgouthaman.microbitble) ([Source code](https://github.com/sumitgouthaman/microbit-ble-mobile)) - Android app that demonstrates communicating with BBC micro:bit over Bluetooth LE and getting sensor data. As an open source app, it's a good example of using Xamaring with the micro:bit.
- [bitty blue](http://www.bittysoftware.com/apps/bitty_blue.html) - iOS and Android app that provides a collection of fun things to do with a BBC micro:bit (or compatible device) and Bluetooth.
- [micro:bit logger](https://play.google.com/store/apps/details?id=nl.defbu.mblogger) - Android app that enables users to log data from the BLE services and export it to a file. 


## ChromeOS应用

- [bitty blue](http://www.bittysoftware.com/apps/bitty_blue.html) - Play with 3D "PolySquiggles", use as a compass, have fun with the buttons, send images or text to the LED display, connect and control electronic circuits, and all via Bluetooth.
- [bitty data logger](http://www.bittysoftware.com/apps/bitty_data_logger.html) - Capture and chart accelerometer, magnetometer and temperature data from your micro:bit's internal sensors over Bluetooth.
- [microbit chrome](https://github.com/Microsoft/microbit-chrome) - Prototype chrome addon that exposes the micro:bit's serial output to webpages like the MakeCode editor.


## Interface Chip

The USB Interface Chip is the microcontroller placed close to the battery connector. It provides the USB mass storage capability to load the micro:bit firmware using the Operating System file explorer.

- [microbit.org Developer Community Info](http://tech.microbit.org/software/daplink-interface/) - This micro:bit Developer Community page contains information about the Interface Chip DAPlink and the USB interface.
- [DAPLink on micro:bit](https://www.mbed.com/en/development/hardware/prototyping-production/daplink/daplink-on-kl26z/) - The DAPLink is the default software running on the Interface Chip, this page contains information, update instructions, and the latest firmware.
- [DAPLink source code](https://github.com/mbedmicro/DAPLink) - Source code for the mbed DAPLink, contains the build configuration for the micro:bit.
- [J-Link OB Firmware](https://www.segger.com/bbc-micro-bit.html) - Offers the same flashing functionality than the DAPLink and expands it to include J-Link debugging.
- [pyOCD](https://github.com/mbedmicro/pyOCD) - Python library for programming and debugging ARM Cortex-M microcontrollers, like the one included in the micro:bit, using the CMSIS-DAP provided by the Interface Chip.
- [DAP.JS](https://github.com/Microsoft/dapjs) - Node.js interface to DAP-CMSIS over USB/HID, meant to provide a subset of functionality of pyOCD.


## 硬件

- [Hardware Design](https://github.com/bbcmicrobit/hardware) - Schematics and bill of materials for the BBC micro:bit.
- [micro:bit Reference Design](https://github.com/microbit-foundation/microbit-reference-design) - Hardware design files for a board 100% binary compatible with the micro:bit. Created to help make your own micro:bit derived designs.
- [micro:bit Badge](https://github.com/make-zurich/micro-bit-badge) - Open Source PCB for the micro:bit with a battery holder, buzzer, extension edge connector and pins breaks out.
- [Eagle micro:bit Edge Part](https://github.com/proto-pic/micro-bit-eagle-libraries) - Eagle librarie from Proto-Pic for the micro:bit edge connectors.
- [Kicad micro:bit Connector](https://github.com/anthonykirby/kicad_microbit_connector) - KiCad component library and footprint library for a micro:bit edge-connector socket.
- [SparkFun Breakout Board](https://github.com/sparkfun/Micro_Bit_Breakout) - Open source files for the SparkFun micro:bit Breakout Board.
- [SparkFun moto:bit](https://github.com/sparkfun/Micro_Bit_Moto_Bit) - Open source files for the SparkFun moto:bit, a board to provide a robotics platform,
- [SparkFun weather:bit](https://github.com/sparkfun/Micro_Bit_Weather_Bit) - Open source files for the SparkFun weather:bit, a board to provide a weather station.
- [SparkFun gamer:bit](https://github.com/sparkfun/Micro_Bit_Gamer_Bit) - Open source files for the SparkFun gamer:bit, a board to provide a game system.


## CAD 和 3D打印

- [Kitronik CAD Resources](https://www.kitronik.co.uk/blog/bbc-microbit-cad-resources/) - BBC micro:bit CAD model from Kitronik.
- [Proto-PIC CAD Resources](https://www.proto-pic.co.uk/micro-bit-resources.html) - Proto-PIC products CAD resources.
- [Microbot Case](http://www.thingiverse.com/thing:1434797) - 3D printed case for the micro:bit in the shape of a robot.
- [micro:bit Stand](http://www.thingiverse.com/thing:2144500) - 3D printed stand for the micro:bit.
- [micro:bit Rover](https://www.myminifactory.com/object/microbit-rover-27013) - 3D printable parts to build a micro:bit robot rover.
- [Micro:Racing](https://www.myminifactory.com/object/micro-racing-18280) - 3D printed wheel case for the micro:bit.
- [Binary Watch](https://www.myminifactory.com/object/binary-watch-15257) - 3D printed watch case and strap for the micro:bit.
- [Micro:bit Compass](https://www.myminifactory.com/object/micro-bit-compass-18994) -3D printed compass case for the micro:bit.
- [A4 folder holder](https://www.myminifactory.com/object/micro-bit-a4-folder-holder-22039) - 3D printed holder to keep your micro:bit in a A4 school folder.
- [mibot drawing robot](https://www.myminifactory.com/object/mibot-drawing-robot-36030) - 3D printed chassis for a painting robot powered by a BBC micro:bit and its motor drive board.


## 项目

All these projects contain steps and resources required for reproduction.

- [Quiz:bit](https://github.com/lancaster-university/quiz-bit) - BBC micro:bit programs and a matching application for providing a quiz-voter-style service using micro:bits as the controls.
- [JUST DO IoT](https://hackaday.io/project/12164-just-do-iot) - Connect the micro:Bit to the LoRaWAN network, includes open source hardware microbit connector board.
- [Micro:Bob](https://hackaday.io/project/8643-microbob) - Simple bipedal robot controlled by a micro:bit.
- Coffee Timer ([1](https://www.norwegiancreations.com/2016/09/coffee-timer-part-1-the-first-prototype-based-on-the-bbc-microbit/), [2](https://www.norwegiancreations.com/2016/10/coffee-timer-part-2-low-power-wireless-on-the-bbc-microbit/), [3](https://www.norwegiancreations.com/2016/11/coffee-timer-part-3-enclosures/)) - Three part article describing how to augment a coffee maker with an micro:bit indicator, options for low power communication, and creating a custom enclosure.
- [Thermal Printer](http://www.suppertime.co.uk/blogmywiki/2016/12/microbit-thermal/) - Connecting and using a Sparkfun thermal till-roll printer.
- [Telescopic Light Sword](https://www.myminifactory.com/object/telescopic-lightsword-with-micro-bit-14598) - Project shows how to make your own Light Sword with the micro:bit, electronics, and 3D printed parts.
- [Micro Simon](http://mrtomsworld.blogspot.co.uk/2017/01/micro-simon.html) - Programming and connecting a micro:bit to a vintage MB Simon game.
- [Connecting a thermal printer to a BBC microbit](http://www.suppertime.co.uk/blogmywiki/2016/12/microbit-thermal/) - Connecting the micro:bit to a thermal till-roll printer to print a random poems or Christmas cracker jokes.
- [Alexa Weather On micro:bit](https://www.hackster.io/chen-tiebiao/weather-on-micro-bit-c79c19) - Creating an Amazon Alexa skill where the current weather can be asked and the result displayed on the micro:bit.
- [BBC Microbit Balloon Tracker](http://www.daveakerman.com/?p=2019) - Making a ballon tracker with a micro:bit connected to GPS and a LoRa transceiver to track and transmit its position.
- [SonicPixels](https://github.com/jrmedd/SonicPixels) - BBC micro:bit and Max frameworks for triggering multiple speakers in a grid arrangment.
- [Little Bug Bit](http://goo.gl/eEFhcy) - Low cost micro:bit buggy.
- [HandShake](https://sites.google.com/site/hardwaremonkey/home/handshake) - Project designed to enable unique gesture recognition for people with limited control of their motion.
- [Mega:Bit](http://www.makerspace-uk.co.uk/megabit/) - Scaled up micro:bit with the 5x5 LED matrix and buttons, connected to a real micro:bit.
- [Scrolling display](https://meanderingpi.wordpress.com/2017/09/16/bbc-microbit-scrolling-display/) - Create a display screen using a number of micro:bits communicating via radio.
- [Ironman Arc Reactor](https://www.kitronik.co.uk/blog/halo-ween-ironman-arc-reactor) - Choose between two different versions (Mk I and Mk II) ready to 3D print and build.

### 项目集

- [microbit.co.uk Site Index](https://www.microbit.co.uk/index) - The microbit.co.uk website contains an extensive list with all their projects and tutorials.
- [hackster micro:bit community](https://www.hackster.io/micro-bit/projects) - This hackster community contains user submitted projects for the micro:bit.
- [MakeCode Projects](https://makecode.microbit.org/projects/) - List of micro:bit projects you can do with the MakeCode editor.
- [Inventorspace micro:bit category](https://invent.sparkfun.com/cwists/category#products=%5B8%5D) - Community by SparkFun with fun projects you can implement in your classroom, school or district.
- [Tinkercademy Projects](https://tinkercademy.com/microbit/) - Collection of projects using the micro:bit and Tinkercademy Tinker Kit.


## 文章

Useful Articles for developing on the micro:bit.

- [Getting Started Microbit & Microsoft’s new www.codethemicrobit.com Environment](https://blogs.msdn.microsoft.com/uk_faculty_connection/2016/08/01/getting-started-microbit-microsofts-new-www-codethemicrobit-com-environment/)
- [Offline C/C++ Development With The Micro:bit](http://www.i-programmer.info/programming/hardware/9654-offline-cc-development-with-the-microbit-.html)
- [Sending 'commands' from a micro:bit over Bluetooth](http://bluetooth-mdw.blogspot.co.uk/2016/07/sending-commands-from-microbit-over.html)
- [Modelling micro:bit data with the Bitty Data Logger App](https://www.stem.org.uk/elibrary/community-resource/289686/modelling-microbit-data-bitty-data-logger-app)
- [Getting Started with the micro:bit Bluetooth IO Pin Service](https://ukbaz.github.io/howto/ubit_ble_profile.html)
- [Using MQTT-SN over BLE with the BBC micro:bit](https://blog.benjamin-cabe.com/2017/01/16/using-mqtt-sn-over-ble-with-the-bbc-microbit)
- [The First Video Game on the BBC Micro:bit [probably]](https://hackernoon.com/the-first-video-game-on-the-bbc-micro-bit-probably-4175fab44da8) - Creating a game for the micro:bit, the MicroPython changes needed to increase performance and a general profile of its resources.
- [Custom BLE services with micro:bit](https://www.hackster.io/pelikhan/custom-ble-services-with-micro-bit-6c9879) - Build your own Bluetooth low energy services and bundle them as PXT/MakeCode blocks that beginners can use.
- [Excel and Micro:Bit - Hacking for fun and creativity!](https://techcommunity.microsoft.com/t5/Excel-Blog/Excel-and-Micro-Bit-Hacking-for-fun-and-creativity/ba-p/63603) - Experiment to have some basic sensor data collected using the micro controller and then visualized in Excel.
- [Writing the second video game for the Micro:bit in Rust](https://hackernoon.com/writing-the-second-video-game-for-the-micro-bit-in-rust-3cd8b5ab22d3) - Updating a micro:bit game and porting it to the Rust language.
- [Build A Klawsome microbit Controlled Tank](https://www.kitronik.co.uk/blog/klawsome-microbit-controlled-tank/) - Tutorial on how to design a build a perspex micro:bit tank.
- [Adding a new module to MicroPython](http://cigdemsengul.blogspot.co.uk/2017/04/offline-development-in-microbit-adding.html) - Article describing an experiment to add a new module into MicroPython for the micro:bit.
- [Become a Time Lord with the BBC micro:bit](https://blog.groklearning.com/become-a-time-lord-with-the-bbc-micro-bit-c4b8b4e2d747) - Using different timing mechanisms to run multiple things in MicroPython.
- [Debugging the micro:bit with pyOCD and GDB](https://docs.mbed.com/docs/mbed-os-handbook/en/5.4/debugging/debugging_microbit/) - Shows how to debug a micro:bit program using PyOCD and GDB.

### 文集

- [MultiWingSpan](http://www.multiwingspan.co.uk/micro.php) - Large collection of examples, instructions, and direction on how to use electronic components.
- [Elecfreaks micro:bit category](https://www.elecfreaks.com/category/micro-bit) - Elecfreaks collection of experiments going through the concepts of using individual sensors or components.
- [SparkFun micro:bit tutorials](https://learn.sparkfun.com/tutorials/tags/microbit) - Collection of tutorials from SparkFun, including comprehensive experiment guides for their kits.
- [BitIO blogs](http://warksjammy.blogspot.co.uk/2017/07/bitio-blogs-in-one-place.html) - Collection of blogs written about using the BitIO Python module to control the micro:bit. 


## 视频

- [MicroMonsters](https://www.youtube.com/channel/UCK2DviDexh_Er2QYZerZyZQ) - YouTube channel with tutorials to learn to code with your family.
- [micro:bit and Bluetooth](https://www.youtube.com/playlist?list=PLYOCnwH2UtBzhJ2nvn_DM3itz6GNVwrDu) - YouTube playlist with Martin Woolley's Bluetooth videos.
- [Video Series from The Maker Movies](https://www.youtube.com/playlist?list=PLD0HD_3AJljXDWoasq2x5gHmkKeV7cc-P) - List of short, introductory videos for anyone wanting to get started with the micro:bit.
- [SparkFun video resources](http://sparkfuneducation.com/video-resources/microbit.html) - Growing list of video resources for the micro:bit.
- [SamCodes YouTube Playlist](https://www.youtube.com/playlist?list=PLumNlyd5JxxegaAVScP7Qm1AXPtJdGBCq) - Video tutorials showing how to  use different electronic components and features of the micro:bit.
- [Fun with Zephyr Project and BBC micro:bit](https://www.youtube.com/watch?v=ZZRbIpVJGns) - This presentation shows how Zephyr empowers the BBC micro:bit devices and its Bluetooth chip to do fun things.


## 书籍

- [micro:bit IoT In C](http://www.iot-programmer.com/index.php/books/micro-bit-iot-in-c)
- [BBC micro:bit - 35 Touch Develop & MicroPython Projects](https://www.elektor.com/bbc-micro-bit-35-touch-develop-micropython-projects)
- [Programming with MicroPython](http://shop.oreilly.com/product/0636920056515.do)
- [Getting Started with the micro:bit](http://shop.oreilly.com/product/0636920115267.do)
- [The Official BBC micro:bit User Guide](http://eu.wiley.com/WileyCDA/WileyTitle/productCd-111938673X.html)
- [Programming the BBC micro:bit](http://simonmonk.org/prog_mb/)


## 教学资源

- [microbit.org Teaching Resources](https://www.microbit.org/teach/)
- [IET micro:bit Teaching Resources](http://faraday.theiet.org/stem-activity-days/bbc-microbit/resources/index.cfm)
- [Code Club micro:bit projects](https://www.codeclubprojects.org/en-GB/microbit/)
- [Make with the micro:bit by Technology Will Save Us](http://make.techwillsaveus.com/bbc-microbit)
- [Grok Learning](https://groklearning.com/microbit/) - Provides an online MicroPython code editor, Blockly visual programming, full micro:bit simulator, curriculum-aligned teaching material and auto-marked problems.
- [Microbit For Primary Schools](http://mb4ps.co.uk) - Fully-customisable scheme of work and resources for use in the primary classroom. 
- [101 Computing BBC micro:bit category](http://www.101computing.net/category/bbc-microbit/) - Computing challenges with the micro:bit to boost your programming skills or spice up your teaching of computer science.
- [Micro:bit Maths](https://microbitmathsblog.wordpress.com) - Blog exploring the BBC micro:bit in mathematics education.
- [micro:bit of Things](https://sites.google.com/view/microbitofthings/) - Notes on micro:bit project ideas for Key Stage 2 and 3.
- [The Brooke Primary School Space Programme](http://www.brooke.norfolk.sch.uk/brooke-space-programme/) - Project page documenting Brooke Primary School pupil's upcoming journey for launching a BBC micro:bit (on its own) into near-space, with experiments and sensor measurements.
- [FunWithMicrobit](https://github.com/MicrobitPolska/FunWithMicrobit) - FunWithMicrobit is a 6 hours workshop made by kids for the kids.
- [Year 7 micro:bit lessons](http://www.jonwitts.co.uk/year-7-microbit) - Lessons used to introduce students to the micro:bit and Python.
- [UCL’s BBC Micro:bit Tutorials](http://microbit-challenges.readthedocs.io/en/latest/) - Tutorial sheets that introduce micro:bit features with practical examples provided to invite students to design solutions to problems.
- [BBC micro:bit and Kodu Interact](https://www.kodugamelab.com/resources/#microbit) - Kodu is a visual programming language made specifically for creating games and allow interaction with the micro:bit.
- [Build A Robot Wars Buggy](https://www.kitronik.co.uk/blog/robot-buggy-part-1-build-robot-wars-buggy-introduction/) - This fun learning resource has been put together to provide teachers with an all in one design and technology challenge that you can set for your students over the course of a term or a year.
- [CPC UCreate Micro:bit resources](http://warksjammy.blogspot.co.uk/2017/04/cpc-ucreate-microbit-resources-all-in.html) - Collection of micro:bit resources made for CPC.
- [Year 7 BBC micro:bit topic](https://bournetocode.com/projects/7-CS-micro/) - BBC micro:bit lessons from Bourne Grammar school.
- [Doctor Who Live Lesson](http://www.bbc.co.uk/programmes/articles/3ydvd6mvhl89cHVJ7F2nmzf/doctor-who-and-the-micro-bit-live-lesson) - The BBC micro:bit will be put to the test at the controls of the TARDIS in this special BBC Live Lesson in collaboration with the team behind Doctor Who.
- [Tackle time and space with Doctor Who and the BBC micro:bit](http://www.bbc.co.uk/programmes/articles/GDNGTpkHJrDJSYMQJbH9f1/tackle-time-and-space-with-doctor-who-and-the-bbc-micro-bit) - Join The Doctor on an adventure of courage, cunning and coding! Part 1: Mission Sonic, Part 2: Mission Decode, and Part 3: Mission Hack.
- [Microsoft 14 Week Curriculum](https://makecode.microbit.org/courses/csintro) - Targeted to middle school grades 6-8 (ages 11-14 years). It is also written for teachers who may not have a Computer Science background, or may be teaching an "Intro to CS" for the first time.
- [micro:bit in science teaching - How clean is my pond](https://community.computingatschool.org.uk/resources/5204) - Using a micro:bit to monitor the level of algal growth in a pond and to control a filter pump.
- [Inventorspace micro:bit category](https://invent.sparkfun.com/cwists/category#products=%5B8%5D) - Community by SparkFun with fun projects you can implement in your classroom, school or district.
- [Strictly micro:bit - BBC Live Lessons](https://www.youtube.com/watch?v=QgEP8aI8Gvw&index=1&list=PLcvEcrsF_9zL-zmL_1-yikUGtsTMo1oO-) - Suitable for teaching ages 11-14. The full BBC Live Lesson exploring the basics of coding, with help from the stars of Strictly Come Dancing and the BBC micro:bit.


## 社区

- [Official Slack Channel](http://tech.microbit.org/get-involved/where-to-find/) - Online form to join this chat group, a great place to discuss and meet more people from the micro:bit community.
- [`@microbit_edu` on twitter](https://twitter.com/microbit_edu)
- [`microbitfoundation` on Facebook](https://www.facebook.com/microbitfoundation)
- [micro:bit Python mailing list](https://mail.python.org/mailman/listinfo/microbit)


## 杂项

- [microbit Fritzing Part](https://github.com/topshed/FritzingParts) - Richard Hayler collection of Fritzing parts contains a model for the micro:bit.
- [micro:bit broadcast](https://microbit-broadcast.embeddedlog.com) - Free newsletter to stay up-to-date with the latest micro:bit news, articles, projects, and resources.
- [micro:bit-o-matic](https://pycomic.github.io/microbit.html) - Easily create micro:bit illustrations with custom LED matrix messages.
- [microbit.org Support](https://support.microbit.org) - The support pages from the micro:bit Foundation is a great source of information, containing an extensive collection of FAQs, articles, and guides. 
- [Radiobit, a BBC Micro:Bit RF firmware](https://github.com/virtualabs/radiobit) - Radiobit is composed of a dedicated Micropython-based firmware and a set of tools allowing security researchers to sniff, receive and send data over Nordic's ShockBurst protocol, Enhanced ShockBurst protocol, Bluetooth Smart Link Layer and sniff raw 2.4GHz GFSK demodulated data.
- [micro:bit Poster](https://www.element14.com/community/servlet/JiveServlet/downloadBody/87638-102-3-368412/microbit24x15.pdf) - Element14 has put together this detailed, beautifully rendered, cross-section micro:bit poster highlighting all of the device's key functions and components.
- [Bluetooth troubleshooting guide](http://www.bittysoftware.com/troubleshooting.html) - Tips on how to solve common and not so common micro:bit Bluetooth problems.
- [Micro World Tour](https://microworldtour.github.io) - Before the micro:bit was released a few went on a tour to the world-wide Python community. A lot of interesting content and ideas on these micro:bit adventures.


## 协议和商标

[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the authors have waived all copyright and related or neighbouring rights to this work.

This projects is not endorsed, sponsored or associated with the BBC. "BBC", "micro:bit", and their logos are trademarks of the BBC.
