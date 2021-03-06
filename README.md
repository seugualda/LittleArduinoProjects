# 282 Little Electronics and Arduino Projects
> Latest addition:sparkles: [FunctionGeneratorKit](./Equipment/FunctionGeneratorKit) - build and test a function generator kit based on the XR-2206 monolithic function generator.


Just my collection of electronics projects, many involving an Arduino in one way or another.
Some are full builds like
[The FretBoard](./FretBoard) (a multi-project build status indicator),
while most are quite trivial breadboard kata, intended to test or explore a single idea.

Many are variations of things found wild on the net, or inspired by ideas from the sources such as:

* [Arduino StackExchange](http://arduino.stackexchange.com/)
* [Electrical Engineering StackExchange](http://electronics.stackexchange.com/)
* [Arduino Playground](http://playground.arduino.cc/)
* [Arduino Cookbook (O'Reilly)](http://www.amazon.com/gp/product/1449313876/ref=as_li_tl?ie=UTF8&camp=1789&creative=390957&creativeASIN=1449313876&linkCode=as2&tag=itsaprli-20&linkId=5F6YF3D5RCEZYXUU)
* and other books from [my electronics bookshelf](https://www.goodreads.com/review/list/17475014-paul?shelf=electronics)

Feel free to borrow liberally, and if you spot any issues do let me know. See the individual projects for credits where due.


## Project Index

LittleArduinoProjects has a new catalog/web site!
It's actually just simple GitHub pages sitting right on top of this repository. Try it out:

[![leap-splash](./catalog/assets/images/leap-splash.png?raw=true)](http://leap.tardate.com/)


## Getting Up and Running

Some projects require additional libraries including FastLED, FlexiTimer2, RadioHead.
A set of such libraries are included as submodules of this repository,
see the [libraries/](./libraries) page for more information on the included libraries and submodule management.

For Arduino projects, I have the Arduino IDE sketchbook location (in preferences) set to the root of this repository.
This makes all the projects available to me in the IDE, and automatically includes libraries
that are linked as git submodules in the [libraries/](./libraries) folder.

If you don't have the Arduino IDE setup this way, libraries can be retrieved with git,
or you can just install them separately as you would any other library.

If you clone this repo, also update the submodules to have them available for compilation:

    $ git submodule update --init

To pull submodule updates later on:

    $ git submodule foreach git pull


## Ye Olde Project Index

Still up to date, but try [the catalog site](http://leap.tardate.com/) instead...


| Project                                                                            | Category/Description                                              |
|------------------------------------------------------------------------------------|-------------------------------------------------------------------|
| [#148 AD9833/BasicDemoCycle](./playground/AD9833/BasicDemoCycle)                   | **Arduino, Oscillators**        run a basic waveform demo with an AD9833 module |
| [#184 AdjustablePulseGenerator](./Electronics101/555Timer/AdjustablePulseGenerator)| **555 Timer, Oscillators**      widely-adjustable square wave generator using the 555 timer |
| [#131 AMFMRadioKit](./Electronics101/AMFMRadioKit)                                 | **RF**                          notes on an AM/FM radio kit build |
| [#143 AM/OpAmpTransmitter](./Electronics101/AM/OpAmpTransmitter)                   | **RF, OpAmp**                   simple AM transmitter with OpAmp carrier/mixer |
| [#132 AMTransmitter/555](./Electronics101/555Timer/AMTransmitter)                  | **RF, 555 Timer**               a simple 555-based AM transmitter |
| [#139 AnalogComparator](./playground/AnalogComparator)                             | **Arduino, Sensor, OpAmp**      test the Atmega328 built-in analog comparator |
| [#020 Arduino Internals](./playground/Internals)                                   | **Arduino**                     report on Arduino Board internals |
| [#100 ArdWinVaders](./playground/OLED/ArdWinVaders)                                | **Arduino, OLED**               an Arduino & OLED version of a classic game |
| [#186 AsyncJKCounter](./Electronics101/AsyncJKCounter)                             | **74xx, Logic**                 an asynchronous 4-bit counter built with JK Flip-Flops |
| [#014 AsyncLedStripEffects](./LEDArrayDemos/AsyncLedStripEffects)                  | **LED Array, Timing, Arduino**  demo effects on the LED strip driven using timer interrupt |
| [#069 ATmegaBreadboard](./playground/ATmegaBreadboard)                             | **Arduino, ATmel**              running an ATMEGA328P-PU on a breadboard  |
| [#099 ATmegaISPShield](./playground/ATmegaISPShield)                               | **Arduino, ATmel**              a DIY ATmega programming shield for using an Arduino as ISP  |
| [#068 ATmegaViaArduinoISP](./playground/ATmegaViaArduinoISP)                       | **Arduino, ATmel**              Programming an ATMEGA328P-PU on a breadboard with Arduino ISP |
| [#275 ATtiny8MHz](./playground/ATtiny8MHz)                                         | **Arduino, ATmel**              how to run an ATtiny85 microprocessor at 8MHz using the internal clock |
| [#126 ATtinyHardwareInterrupt](./playground/ATtinyHardwareInterrupt)               | **Arduino, ATmel**              test hardware interrupts with an ATtiny85 processor on a breadboard |
| [#070 ATtinyWithArduinoISP](./playground/ATtinyWithArduinoISP)                     | **Arduino, ATmel**              Programming an ATTINY85-20PU on a breadboard with Arduino ISP |
| [#253 ATtinyProgrammingShield](./playground/ATtinyProgrammingShield)               | **Arduino, ATmel**              a custom ATtiny programming shield for Arduino ISP |
| [#127 ATtinySleep](./playground/ATtinySleep)                                       | **Arduino, ATmel**              test sleep mode with an ATtiny85 processor on a breadboard |
| [#128 ATtinyTotalSleep](./playground/ATtinyTotalSleep)                             | **Arduino, ATmel**              test a total power shutdown with an ATtiny85 processor on a breadboard |
| [#210 AudioAmps/TDA7297Kit](./Electronics101/AudioAmps/TDA7297Kit)                 | **Audio**                       testing a TDA7297 audio amplifier kit (pump up the jam) |
| [#235 AudioDSP](./playground/AudioDSP)                                             | **Audio, Arduino, DSP, OpAmp**  build and test an arduino DSP circuit based on the pedalSHIELD by electrosmash |
| [#236 AudioDSP/Boost](./playground/AudioDSP/Boost)                                 | **Audio, Arduino, DSP, OpAmp**  arduino DSP boost effect based on the pedalSHIELD by electrosmash |
| [#238 AudioDSP/Crunch](./playground/AudioDSP/Crunch)                               | **Audio, Arduino, DSP, OpAmp**  arduino DSP crunchy distortion effect based on the pedalSHIELD by electrosmash |
| [#237 AudioDSP/Distortion](./playground/AudioDSP/Distortion)                       | **Audio, Arduino, DSP, OpAmp**  arduino DSP simple distortion effect based on the pedalSHIELD by electrosmash |
| [#239 AudioDSP/SuperCrunch](./playground/AudioDSP/SuperCrunch)                     | **Audio, Arduino, DSP, OpAmp**  arduino DSP crunchy symmetrical Schetzen distortion effect based on the pedalSHIELD by electrosmash |
| [#202 AudioLevelIndicatorKit](./Electronics101/AudioLevelIndicatorKit)             | **LM3915, Audio**               an audio level indicator kit based on the LM3915 |
| [#254 AvrHardwarePWM](./playground/AvrHardwarePWM)                                 | **ATmega, ATmel, Arduino, PWM** all about hardware PWM and demonstrating the modes with the Arduino UNO/ATmega328 |
| [#255 AvrHardwarePWM/ATtiny](./playground/AvrHardwarePWM/ATtiny)                   | **ATtiny, ATmel, Arduino, PWM** all about hardware PWM and demonstrating the modes with the ATtiny85 |
| [#217 BasicBuckAvrControl](./playground/BasicBuckAvrControl)                       | **Power, Arduino**              a simple buck converter circuit from first principles |
| [#262 BazzFuss](./Electronics101/GuitarEffects/BazzFuss)                           | **Guitar Effects, Audio**       the Bazz Fuss "chocolate noisette" - a super-minimalist overdrive/distortion/fuzz effect circuit |
| [#133 BidirectionalLevelShifter](./Electronics101/BidirectionalLevelShifter)       | **FET**                         test a basic bi-directional 5/3.3V level shifter circuit |
| [#134 BidirectionalLevelShifterModule](./Electronics101/BidirectionalLevelShifterModule) | **FET**                   test a bi-directional 5/3.3V level shifter module |
| [#093 BJTCurrentSink](./Electronics101/BJTCurrentSink)                             | **BJT, Power**                  test a BJT constant current sink circuit |
| [#094 BJTLongTailPair](./Electronics101/BJTLongTailPair)                           | **BJT, OpAmp**                  test the basic BJT "long-tail" differential amplifier circuit |
| [#138 BJTMonostable](./Electronics101/BJTMonostable)                               | **BJT, RC**                     test a 2-transistor monostable multivibrator |
| [#105 BJTSawTooth](./Electronics101/BJTSawTooth)                                   | **BJT, Oscillators**            testing a simple BJT saw-tooth oscillator |
| [#140 BJTZenerModeEffects](./Electronics101/BJTZenerModeEffects)                   | **BJT, Zener, Oscillators**     playing around with some zener-mode sound effects |
| [#009 Blink](./playground/Blink)                                                   | **LED, Arduino**                the simplest blinking LED, with some electrical measurements thrown in |
| [#030 BlinkPrecision](./playground/BlinkPrecision)                                 | **LED, Timing, Arduino**        use a timer to perform a function on a precise schedule |
| [#269 BoldportClub/cordwood](./BoldportClub/cordwood)                              | **Boldport, PCB Design, LED**  the Cordwood Puzzle evokes an era of stuffing massive components into small spaces without a clear idea of where this is all heading! Introducing the Boldport Club Project #3 |
| [#270 BoldportClub/cordwood/aanimate](./BoldportClub/cordwood/aanimate)            | **Boldport, Cordwood, Arduino** run a demo animation using aaronjasso's Cordwood library |
| [#271 BoldportClub/cordwood/tuner](./BoldportClub/cordwood/tuner)                  | **Boldport, Cordwood, Arduino, Audio** use the Boldport Cuttle & Cordwood as a guitar tuner, with a custom input preamp |
| [#257 BoldportClub/Emergency](./BoldportClub/Emergency)                            | **Boldport, PCB Design, Oscillators** pimp the Boldport Club Emergency kit (Project #2) .. now a LED blinky with 3 passives and a transistor (Esaki Effect) |
| [#263 BoldportClub/ligemdio](./BoldportClub/ligemdio)                              | **Boldport, PCB Design, LED, BJT** an LED tester kit featureing a classic BJT constant current source. From The Boldport Club (Project #8) |
| [#256 BoldportClub/Pease](./BoldportClub/Pease)                                    | **Boldport, PCB Design, LM331** a Bob Pease tribute, LM331 voltage-to-frequency kit from The Boldport Club (Project #1) |
| [#266 BoldportClub/TheCuttle](./BoldportClub/TheCuttle)                            | **Boldport, PCB Design, ATmega, ATmel, Arduino** the most beautiful Arduino-compatible board you will ever see. Another soldering kit from The Boldport Club (Project #6) |
| [#251 BoldportClub/TheLady](./BoldportClub/TheLady)                                | **Boldport, PCB Design**        a ladybird soldering and display kit from The Boldport Club (Project #4) |
| [#277 BoldportClub/Touchy](./BoldportClub/Touchy)                                  | **Boldport, EFM8, Sensors**     Touchy is a capacitive touch input device with on-board Sleepy Bee microcontroller (Boldport Club Project #7) |
| [#162 BoostBuckConverterModule](./Electronics101/BoostBuckConverterModule)         | **Power**                       quick test of an LM2577S/LM2596S Boost/Buck Converter Module |
| [#280 BreadboardTransmitter](./Electronics101/FM/BreadboardTransmitter)            | **FM**                          build a simple 3-stage FM transmitter on a breadboard from a design by dazaro3 |
| [#089 BreatheLamp](./Electronics101/BreatheLamp)                                   | **OpAmp, LED**                  build and test a common LED visual effect circuit |
| [#211 BuckConverterModules](./Electronics101/BuckConverterModules)                 | **Power**                       test a range of low-cost buck converter modules, often using LM2596 |
| [#057 CapacitanceTester](./Electronics101/CapacitanceTester)                       | **LCD, RC, Arduino**            capacitor tester with LCD output |
| [#012 Capacitorial](./Electronics101/Capacitorial)                                 | **RC**                          graphing capacitor discharge with Processing |
| [#206 CD4047/AstableOscillator](./Electronics101/CD4047/AstableOscillator)         | **CMOS, Oscillators**           test the astable operating mode of the CD4047 |
| [#268 ChainBlocks](./playground/ChainBlocks)                                       | **Arduino**                     testing some "Chain Blocks" and demonstrate an XY Plotter block (with an MCP42010 digital potentiometer) by drawing the PrexLab logo on an Oscilloscope |
| [#170 ClapSwitchKit](./Electronics101/ClapSwitchKit)                               | **Oscillators, BJT, Logic Gates** build and analyse a simple clap switch circuit available as a kit |
| [#258 ClapSwitchKit2](./Electronics101/ClapSwitchKit2)                             | **Oscillators, BJT, Logic Gates** practice some Boldport-style soldering on yet-another clap switch kit |
| [#234 CMOSInverterOscillator](./Electronics101/CMOSInverterOscillator)             | **CMOS, Oscillators**           use a CD4096 to generate an oscillating waveform and plot the results |
| [#246 CMOSOscillators](./Electronics101/CMOSOscillators)                           | **CMOS, Oscillators**           testing a 4-pin CMOS oscillator component |
| [#180 ColpittsOscillator](./Electronics101/ColpittsOscillator)                     | **LC, Oscillators**             testing a basic Colpitts Oscillator circuit |
| [#052 Comparator741](./Electronics101/Comparator741)                               | **OpAmp**                       demo LM741 OpAmp comparator mode (with PWM-to-analog side-topic) |
| [#278 ComponentTesterKit](./Equipment/ComponentTesterKit)                          | **Tools, Test Equipment, ATmega**  build and evaluate a popular ATMEAG328-based component tester kit |
| [#136 CounterModule](./playground/CounterModule)                                   | **CMOS, Arduino**               a general-purpose CD4017 counter module |
| [#141 CrystalTester](./Electronics101/CrystalTester)                               | **RF, Oscillators**             a Colpitts Oscillator circuit for testing crystal oscillators with a frequency counter |
| [#168 CurrentSensorModule](./playground/CurrentSensorModule)                       | **Sensors, Arduino**            test an ACS712 voltage sensor module with display on a 5110 LCD |
| [#130 DarlingtonTouchSwitch](./Electronics101/DarlingtonTouchSwitch)               | **Sensors, BJT**                test a Darlington-pair touch switch |
| [#229 Dice](./Electronics101/555Timer/Dice)                                        | **555 Timer, CMOS**             a 555/4017-based dice circuit with slow-down and auto power-off |
| [#240 DigitalInputWithAnalogPins](./playground/DigitalInputWithAnalogPins)         | **Arduino**                     demonstrate how analog pins can also be used as a digital GPIO |
| [#259 DigitalPots/M62429](./Electronics101/DigitalPots/M62429)                     | **Arduino, Digital Pot, M62429** control the M62429 dual channel volume control with an Arduino |
| [#261 DigitalPots/MCP4017](./Electronics101/DigitalPots/MCP4017)                   | **Arduino, Digital Pot, MCP4017** control the MCP4017 single 7-Bit I²C digital potentiometer with an Arduino |
| [#264 DigitalPots/MCP42010](./Electronics101/DigitalPots/MCP42010)                 | **Arduino, Digital Pot, MCP42010** control the MCP42010 dual 10kΩ digital potentiometer with an Arduino and hardware SPI |
| [#110 DiodeLogic/AND](./Electronics101/DiodeLogic/AND)                             | **Diode, Logic Gates**          test the basic diode-logic AND gate |
| [#109 DiodeLogic/OR](./Electronics101/DiodeLogic/OR)                               | **Diode, Logic Gates**          test the basic diode-logic OR gate |
| [#201 DoorbellKit](./Electronics101/555Timer/DoorbellKit)                          | **555 Timer, Oscillators**      another two-tone doorbell using a 555 timer oscillator |
| [#219 DS18S20/OneWireReading](./playground/DS18S20/OneWireReading)                 | **Sensors, Arduino**            basic interrogation of a DS18S20 using 1-wire protocol |
| [#166 DS3231RTC/TimeDemo](./playground/DS3231RTC/TimeDemo)                         | **RTC, Arduino**                prints the system time synced from the RTC to the serial output |
| [#188 EEPROM/AT24C02/BasicReadWrite](./playground/EEPROM/AT24C02/BasicReadWrite)   | **EEPROM, Arduino**             basic read/write operations to external EEPROM (AT24C02) with the Wire library |
| [#051 El Jarabe Tapatío](./playground/JarabeTapatio)                               | **Audio, Arduino**              play The Mexican Hat Dance on a piezo buzzer with LM 386 amplification |
| [#038 ElectretADC](./playground/ElectretADC)                                       | **Audio, Arduino**              convert electret signal to a full range analog input with an LM324 preamp and plot the raw and aplified signals |
| [#037 ElectretTrigger](./playground/ElectretTrigger)                               | **Sensors, Audio, OpAmp, Arduino** uses an electret microphone and LM324 amplifier to trigger action when over audio threshold |
| [#088 ElectronicClockKit](./Electronics101/ElectronicClockKit)                     | **LCD, Kit**                    build and investigate a commercially available "electronic clock" kit |
| [#194 ESP8266/DIYDevBoard](./playground/ESP8266/DIYDevBoard)                       | **ESP8266**                     a DIY devboard for an ESP-01 ESP8266 |
| [#154 ESP8266/SerialTest](./playground/ESP8266/SerialTest)                         | **ESP8266**                     first test of an ESP8266 module - serial communication to the SoC |
| [#155 ESP8266/SerialTest/ruby](./playground/ESP8266/SerialTest/ruby)               | **ESP8266, ruby**               exercising ESP8266 serial communications with Ruby |
| [#274 FY3200S](./Equipment/FY3200S)                                                | **Tools, Test Equipment**       testing out the Feeltech FY3200S digital function generator |
| [#225 FQ777-954/TearDown](./Kinetics/FQ777-954/TearDown)                           | **Drones, RF**                  teardown an FQ777-954 nano drone and figure out as much of the technical design as possible |
| [#223 Fritzing Parts](./FritzingParts)                                             | **EDA**                         my collection of custom Fritzing Parts |
| [#207 FrequencyCounter](./Electronics101/FrequencyCounter)                         | **CMOS, Oscillators**           test a CMOS frequency counter circuit with 100Hz - 5MHz range |
| [#018 FretBoard](./FretBoard)                                                      | **LED Array, Arduino**          a multi-project build status indicator, that pulls software build status from the net and animates the status of up to 24 projects with an LED array |
| [#053 FunctionGenerator324](./Electronics101/FunctionGenerator324)                 | **OpAmp, Oscillators**          LM324 configured as a low-frequency square, triangle, sine, and cosine function generator |
| [#282 FunctionGeneratorKit](./Equipment/FunctionGeneratorKit)                      | **Oscillators, Tools, XR2206**  build and test a function generator kit based on the XR-2206 monolithic function generator |
| [#061 Gates - RS Flip Flop](./Electronics101/RSFlipFlop)                           | **Logic Gates, BJT**            Set/Reset flip-flop with BJTs |
| [#062 Gates - RS Flip Flop with Arduino](./Electronics101/RSFlipFlopFlipper)       | **Logic Gates, BJT, Arduino**   Set/Reset flip-flop with BJTs, under Arduino control and monitoring |
| [#077 Gates - RS Flip Flop/NOR Latch](./Electronics101/RSFlipFlop_NORLatch)        | **Logic Gates, 74xx**           Set/Reset flip-flop implemented with NOR gates |
| [#220 GccToolchain](./playground/GccToolchain)                                     | **avr-lib, avrdude**            programming an Arduino with C and a command line |
| [#245 GeneralCurveTracer](./Electronics101/GeneralCurveTracer)                     | **BJT, Oscillators**            test a DC-powered general curve tracer circuit |
| [#241 GeneralPurpose358](./Electronics101/AudioAmps/GeneralPurpose358)             | **OpAmp, Audio**                test a general-purpose LM358 amplifier circuit |
| [#050 Girabot](./Girabot)                                                          | **Sensors, OpAmp, Arduino**     EE40LX Electronic Interfaces robot project |
| [#098 GuitarHeadphoneAmp](./Electronics101/AudioAmps/GuitarHeadphoneAmp)           | **OpAmp, Audio**                an LM386 fixed-gain guitar headphone amp |
| [#249 GuitarPracticeAmp](./Electronics101/AudioAmps/GuitarPracticeAmp)             | **OpAmp, Audio**                single-channel 10W guitar practice amplifier based on the TDA2050 |
| [#198 HallEffectSwitch](./Electronics101/HallEffectSwitch)                         | **Sensors**                     testing a Hall effect switch |
| [#005 HeartQuotes](./playground/HeartQuotes)                                       | **LCD, Ethernet, Arduino**      press a button to get a quote from the net and display on an LCD |
| [#142 HighFrequencyOpAmpOscillators](./Electronics101/HighFrequencyOpAmpOscillators) | **OpAmp, Oscillators**         how fast can you push an Op-Amp oscillator? |
| [#043 HitTheLights](./playground/HitTheLights)                                     | **LCD, Human Input, Arduino**   simple LED game with LCD output and interrupt-driven button input |
| [#203 HomopolarMotor](./Kinetics/HomopolarMotor)                                   | **Kinetics**                    build a basic homopolar motor |
| [#146 InvertingChargePump](./Electronics101/555Timer/InvertingChargePump)          | **555 Timer, Power**            test an inverting charge pump circuit based on a 555 timer |
| [#006 It's Better With Bacon](./playground/BetterWithBacon)                        | **LCD, Arduino**                simple LCD test |
| [#056 JoystickServoControl](./playground/JoystickServoControl)                     | **Human Input, Arduino**        controlling two servos with a joystick |
| [#227 KnightRider](./Electronics101/555Timer/KnightRider)                          | **555 Timer, CMOS, LED**        the familiar "Knight-Rider" LED circuit using a 555 and 4017 |
| [#085 Lcd5110/BareBack](./playground/Lcd5110/BareBack)                             | **LCD, Arduino**                driving a Nokia 5110 LCD Display with an Arduino and the raw command set |
| [#149 Lcd5110/JuliansU8glibDemo](./playground/Lcd5110/JuliansU8glibDemo)           | **LCD, Arduino**                quick test drive of Julian Ilett's 5110 LCD demo with the u8glib library |
| [#195 LCResonator](./Electronics101/LCResonator)                                   | **Oscillators, LC**             measure the resonant frequency of an LC circuit or inductance of an inductor  |
| [#034 LDRComparator](./Electronics101/LDRComparator)                               | **Sensors, OpAmp, Arduino**     low-light/proximity Trip Detector demonstration using LM324 and LDR/Wheatstone Bridge sensor |
| [#047 LDRStereoTripDetector](./Electronics101/LDRStereoTripDetector)               | **OpAmp**                       demo LM324 OpAmp as threshold trigger for stereo LDR/Wheatstone Bridge sensor |
| [#058 Led4Digit7Segment](./playground/Led4Digit7Segment)                           | **7-Segment, Arduino**          overview of driving a 4-digit 7-segment display |
| [#080 Led4Digit7Segment/DoubleShift](./playground/Led4Digit7Segment/DoubleShift)   | **7-Segment, 74xx, Arduino**    driving a 4-Digit 7-Segment display with only 3 pins, using two 74HC595 shift registers and some NPN BJTs |
| [#081 Led4Digit7Segment/DoubleShiftWithFETs](./playground/Led4Digit7Segment/DoubleShiftWithFETs) | **7-Segment, 74xx, Arduino** driving a 4-Digit 7-Segment display with only 3 pins, using two 74HC595 shift registers and some n-channel FETs |
| [#078 Led4Digit7Segment/SingleShift](./playground/Led4Digit7Segment/SingleShift)   | **7-Segment, 74xx, Arduino**    driving a 4-digit 7-segment display with a shift register and a few BJTs |
| [#199 LED7Segment/CD4026BucketBrigade](./playground/LED7Segment/CD4026BucketBrigade) | **7-Segment, CMOS, Arduino**  a CD4026 bucket-brigade for driving multiple 7-segment displays |
| [#196 LED7Segment/CD4026Drive](./playground/LED7Segment/CD4026Drive)               | **7-Segment, CMOS, Arduino**    driving a 7-segment display with CD4026 Counter |
| [#001 LED7Segment/DirectDrive](./playground/LED7Segment/DirectDrive)               | **7-Segment, Arduino**          test a 7-segment common cathode display |
| [#177 LED7Segment/ShiftDrive](./playground/LED7Segment/ShiftDrive)                 | **7-Segment, 74xx, Arduino**    test control of a 7-segment display via a 74HC595 shift register |
| [#178 LED7Segment/ShiftDriveModule](./playground/LED7Segment/ShiftDriveModule)     | **7-Segment, 74xx, Arduino, PCB** a custom 7-segment display module PCB with 74HC595 shift register interface |
| [#189 LED7Segment/ShiftDriveSPI](./playground/LED7Segment/ShiftDriveSPI)           | **7-Segment, 74xx, Arduino, SPI** using SPI to control a 7-segment display via a 74HC595 shift register |
| [#007 LEDArrayDemos](./LEDArrayDemos)                                              | **LED Array, Arduino**          Intro and Setup.. I bought some [WS2811-based LED Strips](http://www.aliexpress.com/item/IP68-12mm-WS2811-as-WS2801-led-pixel-module-IP68-waterproof-DC5V-full-color-RGB-50pcs-a/1932649085.html) with a specific project in mind. But first, need to get them working... |
| [#003 LEDChaser](./playground/LedChaser)                                           | **LED, Arduino**                blinks a series of 12 LEDs in a coninuous loop |
| [#103 LedControlDemo](./playground/LED8x8/LedControlDemo)                          | **8x8 LED, Arduino**            test driving and LED matrix with the LedControl library |
| [#173 LEDCubes/Mini4](./playground/LEDCubes/Mini4)                                 | **LED, 74xx, Arduino**          a mini 64 LED cube with an Atmel328 and 3 x 74HC595 register interface |
| [#231 LEDDimmer/CurrentRegulator](./Electronics101/LEDDimmer/CurrentRegulator)     | **LED, Power**                  test a current-regulator style LED dimmer circuit |
| [#232 LEDDimmer/555PWM](./Electronics101/LEDDimmer/555PWM)                         | **LED, Power, 555 Timer**       test a PWM LED dimmer circuit using a 555 timer |
| [#067 LEDLamp](./Electronics101/LEDLampAC)                                         | **Power, LED**                  build and analyse a commercial LED lamp kit with capacitive power supply |
| [#209 LedPanelDisplay72R02](./playground/LedPanelDisplay72R02)                     | **LED, Arduino**                test a 7-digit & 7-status indicator LED display |
| [#224 LEDStrobeKit](./Electronics101/LEDStrobeKit)                                 | **LED, 555 Timer, CMOS**        build and analyse a common LED strobe kit |
| [#079 LedTemperatureDisplay](./playground/LedTemperatureDisplay)                   | **Sensors, LM35, 7-Segment, Arduino** measure ambient temperature using LM35 and display with a 4-digit 7-segment LED unit |
| [#179 LEDx16Module](./playground/LEDx16Module)                                     | **74xx, SMD, Arduino**          a custom 16 LED SMD PCB with 74HC595 shift register interface |
| [#065 LevelIndicatorLM3915](./playground/LevelIndicatorLM3915)                     | **LM3915, Arduino**             Driving an LM3915 10-segment display with a single Arduino pin |
| [#010 LightOrNot](./playground/LightOrNot)                                         | **Sensors, Arduino**            uses an LDR to adjust the blink rate of an LED |
| [#095 LittleGem/A386](./Electronics101/AudioAmps/LittleGem)                        | **OpAmp, Audio**                a basic Smokey-inspired LM386 guitar power amp |
| [#191 LowVoltageGlowingLEDs](./Electronics101/LowVoltageGlowingLEDs)               | **BJT, LED, Oscillators, Power** a dual-LED "glowing" oscillator from a 1.5V supply |
| [#160 LM324/SplitterBuffer](./Electronics101/LM324/SplitterBuffer)                 | **OpAmp**                       demonstrate load-independance of an LM324 buffer and signal splitter |
| [#101 MaxRawDemo](./playground/LED8x8/MaxRawDemo)                                  | **8x8 LED, Arduino**            drive an 8x8 LED Matrix with a MAX7219 chip an raw SPI commands |
| [#040 MeLEDy](./Electronics101/MeLEDy)                                             | **Audio**                       use an electret microphone to light a series of LEDs in proportion to volume |
| [#252 MessageWaiting](./Electronics101/555Timer/MessageWaiting)                    | **LED, 555 Timer**              two-LED flasher with a 555 and minimal components - turned into a "message waiting" indicator with some free-wired SMD construction |
| [#230 MinimalLCOscillator](./Electronics101/MinimalLCOscillator)                   | **LC, Oscillators**             test an LC oscillator of just 5 components |
| [#150 ML741](./Electronics101/ML741)                                               | **OpAmp**                       an LM741-style OpAmp built with discrete components |
| [#151 ML741/Comparator](./Electronics101/ML741/Comparator)                         | **OpAmp**                       test a comparator circuit with the ML741 discrete component opamp |
| [#158 ML741/Inverter](./Electronics101/ML741/Inverter)                             | **OpAmp**                       test an inverter circuit using the ML741 discrete component opamp |
| [#159 ML741/InvertingAmplifier](./Electronics101/ML741/InvertingAmplifier)         | **OpAmp**                       test an inverting amplifier circuit using the ML741 discrete component opamp |
| [#161 ML741/NonInvertingAmplifier](./Electronics101/ML741/NonInvertingAmplifier)   | **OpAmp**                       test a non-inverting amplifier circuit using the ML741 discrete component opamp |
| [#157 ML741/VoltageFollower](./Electronics101/ML741/VoltageFollower)               | **OpAmp**                       test a voltage follower/buffer circuit with the ML741 discrete component opamp |
| [#082 MobileRFDetectorKit](./Electronics101/EMRDetection/MobileRFDetectorKit)      | **RF**                          build and investigate a commercially available "mobile phone signal" detector kit |
| [#017 Monostable](./Electronics101/555Timer/Monostable)                            | **555 Timer**                   basic monostable mode using an Arduino and processing to plot the output |
| [#075 Monostable122](./Electronics101/Monostable122)                               | **74xx TTL**                    simple pulse trigger using 74LS122 monostable with external timing configuration |
| [#076 MonostablePulseExtender](./playground/MonostablePulseExtender)               | **74xx TTL, Arduino**           test the behaviour of a 74LS122 monostable with external timing configuration and plot the results with an Arduino |
| [#046 MotorControlPWM](./playground/MotorControlPWM)                               | **Motors, Arduino**             tests PWM speed control of a DC motor driven by an Arduino |
| [#218 MPU6050/AccelGyroTest](./playground/MPU6050/AccelGyroTest)                   | **Sensors, MPU-6050, Arduino**  first test of an Invensense MPU-6050 3-Axes Accelerometer Gyroscope Module |
| [#190 MultiSlaveSPI](./playground/MultiSlaveSPI)                                   | **SPI, Arduino**                using SPI to control multiple devices that support an SPIish interface |
| [#226 MusicBoxKit](./Electronics101/MusicBoxKit)                                   | **Music, Arduino**              build and test a Music Box kit, and run a demonstration under Arduino control |
| [#156 MSO5074FG_unboxing](./Equipment/MSO5074FG_unboxing)                          | **Tools, Test Equipment, Oscilloscope** unboxing and first tests of a Hantek MSO5074FG oscilloscope |
| [#036 NonInverting324](./Electronics101/NonInverting324)                           | **OpAmp**                       demo LM324 OpAmp non-inverting DC gain mode |
| [#072 NOR7402](./Electronics101/NOR7402)                                           | **74xx TTL, Arduino**           demo the 74LS02 Quad 2-input NOR gate with an Arduino |
| [#114 NORGateOscillator](./Electronics101/NORGateOscillator)                       | **74xx TTL, Oscillators, Arduino** test a low-speed square wave oscillator using NOR gates |
| [#176 nRF24Breakout](./Electronics101/nRF24Breakout)                               | **nRF24, PCB**                  a simple PCB breadboard adapter for 8-pin nRF24 modules |
| [#187 nRF24/PingPong](./playground/nRF24/PingPong)                                 | **nRF24, Arduino**              two Arduino's entertaining themselves with a game of "ping pong" over nRF24L01+ 2.4GHz RF |
| [#087 OLED/SSD1306BareBack](./playground/OLED/SSD1306BareBack)                     | **OLED, Arduino**               driving a monochrome 128x64 OLED Display with an Arduino and the raw command set |
| [#086 OLED/SSD1306WithAdaFruitLibraries](./playground/OLED/SSD1306WithAdaFruitLibraries) | **OLED, Arduino**         running the AdaFruit example program with a monochrome 128x64 OLED Display |
| [#122 OpAmpTimer](./Electronics101/OpAmpTimer)                                     | **OpAmp, Timer**                testing an OpAmp timer switch |
| [#213 OSHChip/blinky](./OSHChip/blinky)                                            | **ARM, OSHChip**                first tests of the OSHChip nRF51822-CFAC-A0 in DIP16 packaging |
| [#214 OSHChip/GccToolchain](./OSHChip/GccToolchain)                                | **ARM, gcc, OSHChip**           can I build a program for the OSHChip using the gcc toolchain and Nordic Semi SDK on MacOSX? |
| [#216 OSHChip/LEDx16Module](./OSHChip/LEDx16Module)                                | **OSHChip, SPI**                driving an SPI LED module with the OSHChip |
| [#215 OSHChip/YottaToolchain](./OSHChip/YottaToolchain)                            | **ARM, gcc, yotta, OSHChip**    build a simple program using the Official Yotta target for OSHChip and gcc on MacOSX |
| [#121 PeakDetector](./Electronics101/PeakDetector)                                 | **OpAmp, RC**                   test an OpAmp-based peak detector circuit |
| [#247 pedalShieldUno](./playground/pedalShieldUno)                                 | **DSP, Guitar, Arduino**        build and test a genuine pedalSHIELD UNO Arduino-based guitar effects pedal |
| [#250 pedalShieldUno/AudioDSP](./playground/pedalShieldUno/AudioDSP)               | **DSP, Guitar, Arduino**        test and develop the AudioDSP library for programming the pedalSHIELD Uno |
| [#248 PierceGateOscillator](./Electronics101/PierceGateOscillator)                 | **Oscillators, Crystal**        build and test a 4.27 MHz Pierce Gate Oscillator circuit using a 74LS14 schmitt inverter |
| [#242 PierceOscillator](./Electronics101/PierceOscillator)                         | **Oscillators, Crystal**        test a Pierce Oscillator made with a minimum of components |
| [#090 PlotNValues](./playground/PlotNValues)                                       | **Arduino, Processing**         generic script to sample up to 6 analog inputs and stream the data to serial in ASCII format for plotting with Processing |
| [#183 PolarityTester](./Electronics101/PolarityTester)                             | **Inverter, CMOS**              demonstrate a polarity-testing circuit |
| [#193 PovShakeStickKit](./Electronics101/PovShakeStickKit)                         | **8051, LED**                   build and investigate an AT89S52-based "shake stick" kit |
| [#165 Power2662Inverter](./Electronics101/Power2662Inverter)                       | **Power**                       test a negative 5V power supply using the LM2662 Switched Capacitor Voltage Converter |
| [#026 Power317](./Electronics101/Power317)                                         | **Power**                       test/graph an adjustable voltage supply built with the LM317 Adjustable Regulator |
| [#092 Power317CC](./Electronics101/Power317CC)                                     | **Power**                       test a constant current power supply built with the LM317 |
| [#027 Power7805](./Electronics101/Power7805)                                       | **Power**                       test and graph a voltage supply built with an LM7805 5V Regulated Supply |
| [#153 PowerAMS1117](./Electronics101/PowerAMS1117)                                 | **Power**                       test an AMS1117 3.3V linear regulator |
| [#060 PowerBreadboard5V](./Electronics101/PowerBreadboard5V)                       | **Power**                       custom regulated 5V power supply module for standard breadboard |
| [#152 PowerLD1117](./Electronics101/PowerLD1117)                                   | **Power**                       test an LD1117 3.3V linear regulator |
| [#028 PowerMB102](./Electronics101/PowerMB102)                                     | **Power**                       demo and test a commercial 3.3/5V MB102 breadboard power supply unit |
| [#182 PowerSupply317Kit](./Electronics101/PowerSupply317Kit)                       | **Power**                       build and test a mains-powered 1.25V-12V DC LM317 power supply kit |
| [#029 PowerZener](./Electronics101/PowerZener)                                     | **Power**                       test and graph a power supply regulated with a 1N4733 zener diode |
| [#019 Popcorn](./playground/Popcorn)                                               | **Audio, Arduino**              How to make a piezo buzzer even more annoying? Make it play popcorn! |
| [#004 Pushbutton LED switch](./playground/PushbuttonLED)                           | **LED, Arduino**                Momentary push button switch is used to toggle the LED on and off |
| [#233 PWM/GeneralPurposeHighSideController](./Electronics101/PWM/GeneralPurposeHighSideController) | **PWM, 555 Timer, Oscillators, Power**  build and test a general-purpose high-side PWM controller |
| [#025 Quad Latch](./Electronics101/QuadLatch)                                      | **74xx TTL**                    graph the basic operation of the 74LS75 4-bit bistable latch |
| [#073 QuadNOR](./Electronics101/QuadNOR)                                           | **74xx TTL, Arduino**           demo simple cascading NOR gate logic with the 74LS02 and an Arduino |
| [#115 R2RDAC](./playground/R2RDAC)                                                 | **Arduino**                     build and test a 16-bit R2R-ladder digital to analog converter with shift register interface |
| [#035 RangeFinder](./playground/RangeFinder)                                       | **Sensors, Arduino**            proximity/distance measurement with an HC-SR04 untrasonic ranging module |
| [#049 RCOscillator](./Electronics101/RCOscillator)                                 | **BJT, RC, Oscillators**        simple RC/transistor multistable vibrator |
| [#129 RelaxationJouleThief](./Electronics101/RelaxationJouleThief)                 | **Power, RLC, Oscillators**     test a "joule thief" circuit based on a relaxation oscillator |
| [#055 RelayControlTest](./playground/RelayControlTest)                             | **Servo, Arduino**              quick test to drive a motor with a common relay using NPN switching circuit under Arduino control |
| [#054 RelayModuleTest](./playground/RelayModuleTest)                               | **Servo, Arduino**              quick test of a common relay board to switch a motor under Arduino control |
| [#024 ResistorTransistorLogic/AND](./Electronics101/ResistorTransistorLogic/AND)   | **BJT, RTL, Logic Gates**       test the basic resistor-transistor logic AND gate  |
| [#023 ResistorTransistorLogic/NAND](./Electronics101/ResistorTransistorLogic/NAND) | **BJT, RTL, Logic Gates**       test the basic resistor-transistor logic NAND gate  |
| [#111 ResistorTransistorLogic/NOR](./Electronics101/ResistorTransistorLogic/NOR)   | **BJT, RTL, Logic Gates**       test the basic resistor-transistor logic NOR gate  |
| [#013 ResistorTransistorLogic/NOT](./Electronics101/ResistorTransistorLogic/NOT)   | **BJT, RTL, Logic Gates**       test the basic resistor-transistor logic NOT gate (Inverter) |
| [#112 ResistorTransistorLogic/OR](./Electronics101/ResistorTransistorLogic/OR)     | **BJT, RTL, Logic Gates**       test the basic resistor-transistor logic OR gate |
| [#221 ResistorTransistorLogic/XOR](./Electronics101/ResistorTransistorLogic/XOR)   | **BJT, RTL, Logic Gates**       test the basic resistor-transistor logic XOR gate/XOR |
| [#124 RFDetectorProbe](./Electronics101/EMRDetection/RFDetectorProbe)              | **RF**                          a simple RF detector mounted in a pen |
| [#169 RGBLedModule](./playground/RGBLedModule)                                     | **LED, Arduino**                demo an RGB LED module |
| [#107 RingCounter](./Electronics101/RingCounter)                                   | **CMOS, 555 Timer**             test the classic CD4017 walking-ring counter |
| [#108 RingCounterController](./playground/RingCounterController)                   | **CMOS, Arduino**               control the classic CD4017 walking-ring counter with an Arduino |
| [#144 RingOscillator](./Electronics101/RingOscillator)                             | **74xx TTL, Oscillators**       test an oscillator built with a 74LS14 Inverter chip |
| [#063 RFSwitch](./Electronics101/RFSwitch)                                         | **RF, OpAmp**                   simple remote control switch with 433Mhz transmitter/receiver and some analog signal processing |
| [#064 RFSwitchASK](./playground/RFSwitchASK)                                       | **RF, ASK, Arduino**            data communications using ASK protocol over 433Mhz RF transmitter and receiver set |
| [#008 RGBCalibrate](./LEDArrayDemos/RGBCalibrate)                                  | **LED Array, Arduino**          quick test to make sure LEDs are correctly addressable and their color can be set correctly |
| [#118 RotaryEncoderMethods](./playground/RotaryEncoderMethods)                     | **Sensor, Arduino**             finding the best method for reading a rotary-encoder |
| [#119 RotaryEncoderModule](./playground/RotaryEncoderModule)                       | **Sensor, 8x8 LED, Arduino**    testing a Rotary Encoder module controlling an LED 8x8 display |
| [#084 RouletteKit](./Electronics101/555Timer/RouletteKit)                          | **555 Timer**                   build and examine the workings of a commercial 555 Roulette kit |
| [#104 Ruby](./Electronics101/AudioAmps/Ruby)                                       | **OpAmp, Audio**                a version of the runoffgroove Ruby LM386 guitar amp |
| [#192 Sagrada Família](./Kraft/SagradaFamilia)                                     | **LED, Kraft**                  a paper model with some LED effects |
| [#272 Saike909D](./Equipment/Saike909D)                                            | **Tools, Test Equipment**       unboxing and initial review of the Saike 909D 3-in-1 hot air rework station |
| [#260 SaleaeLogic](./Equipment/SaleaeLogic)                                        | **Tools, Test Equipment, Logic Analyzer**  checking out a second-hand Saleae Logic (24 MS/s, 8 channel USB logic analyzer - that works on a Mac!!) |
| [#021 Schmitt Inverter](./Electronics101/SchmittInverter)                          | **74xx TTL**                    graph the basic operation of the 74LS14 Hex Inverter with Schmitt Trigger Inputs |
| [#172 SCRLatch](./Electronics101/SCRLatch)                                         | **SCR, Thyristor**              exploring the behaviour of low-power silicon controlled rectifiers (SCR) |
| [#042 ServoTest](./playground/ServoTest)                                           | **Servo, Arduino**              test the positioning accuracy of a servo motor driven by an Arduino |
| [#041 Shifty](./playground/Shifty)                                                 | **LED, 74xx, Arduino**          drive 8 LEDs with 3 pins using a 74HC595 shift register |
| [#044 SimpleChime](./Electronics101/555Timer/SimpleChime)                          | **555 Timer**                   play a sound for a fixed duration when a button is pressed |
| [#120 SimplePeakDetector](./Electronics101/SimplePeakDetector)                     | **RC**                          test the basic diode-RC peak detector circuit |
| [#045 SimpleSiren](./Electronics101/555Timer/SimpleSiren)                          | **555 Timer**                   classic timer circuit producing a two-tone oscillation |
| [#208 SingleStageTransmitterKit](./Electronics101/FM/SingleStageTransmitterKit)    | **FM**                          build a simple single-stage FM transmitter kit |
| [#279 SingleStageTransmitterKit2](./Electronics101/FM/SingleStageTransmitterKit2)  | **FM**                          build and tweak/tune another simple single-stage FM Transmitter Kit |
| [#171 SMDPracticeBoards](./Electronics101/SMDPracticeBoards)                       | **SMD, CMOS, 555 Timer**        a collection of notes, kits and resources for hand-soldering surface mount devices |
| [#096 Smokey](./Electronics101/AudioAmps/Smokey)                                   | **Amp, Audio**                  quick build of a Smokey-like LM386 guitar power amp |
| [#102 SolenoidControl](./playground/SolenoidControl)                               | **Solenoid, Arduino**           controlling a mini solenoid with an Arduino |
| [#117 SolenoidDIY](./Electronics101/SolenoidDIY)                                   | **Solenoid, Arduino**           build and test a basic electromechanical solenoid |
| [#200 SolenoidMotor](./Kinetics/SolenoidMotor)                                     | **Solenoid**                    a single-cylinder mini-solenoid engine |
| [#016 Square Wave - 555](./Electronics101/555Timer/AstableOscillator)              | **555 Timer, Oscillators**      using a 555 timer to generate a square wave and an Arduino and processing to plot the output |
| [#039 Square Wave - LM324](./Electronics101/LM324Oscillator)                       | **OpAmp, Oscillators**          using an LM324 OpAmp to generate a square wave |
| [#022 Square Wave - Schmitt](./Electronics101/SchmittOscillator)                   | **74xx TTL, Oscillators**       using an 74LS14 Hex Inverter with Schmitt Trigger Inputs to generate a square wave |
| [#222 StairStepGenerator](./Electronics101/StairStepGenerator)                     | **OpAmp, 555 Timer, Oscillators**  generate a stair-step waveform with analog components |
| [#212 StayCreative](./Electronics101/StayCreative)                                 | **Audio, LED**                  an audio level VU meter driving a custom LED sign |
| [#048 StereoLightTrigger](./playground/StereoLightTrigger)                         | **Sensors, Arduino**            demo an interrupt-driven method for responding to LDR light threshold triggers |
| [#185 StirlingEngineHB13](./Kinetics/StirlingEngineHB13)                           | **Kinetics**                    building the Böhm Stirling-Technik HB13 Small Bonsai engine |
| [#015 StripTease](./LEDArrayDemos/StripTease)                                      | **LED Array, Arduino**          demo a range of effects on the LED strip |
| [#123 SuperheterodyneReceiverKit](./Electronics101/SuperheterodyneReceiverKit)     | **RF**                          build and analyse a basic commercial radio recevier kit |
| [#066 Switch - NFET](./Electronics101/SwitchNFET)                                  | **MOSFET**                      small-signal n-channel MOSFET switch with turn-off delay |
| [#116 Switch - NJFET](./Electronics101/SwitchNJFET)                                | **JFET, Arduino**               switch an independent power source using an Arduino and n-channel JFET |
| [#032 Switch - NPN](./Electronics101/SwitchNPN)                                    | **BJT**                         small-signal digital switch with NPN BJT |
| [#106 Switch - PFET](./Electronics101/SwitchPFET)                                  | **MOSFET**                      small-signal p-channel MOSFET switch with turn-on delay |
| [#091 Switch - PJFET](./Electronics101/SwitchPJFET)                                | **JFET, Arduino**               switch an independent power source using an Arduino and p-channel JFET |
| [#033 Switch - PNP](./Electronics101/SwitchPNP)                                    | **BJT**                         small-signal digital switch with PNP BJT |
| [#243 Switches](./Electronics101/Switches)                                         | **Switches**                    Notes on miscellaneous mechanical switches used in electrical circuits |
| [#244 Switches/DPDT](./Electronics101/Switches/DPDT)                               | **Switches**                    all about double-pole, double-thow (DPDT) toggle switches |
| [#175 SwitchSoftLatch](./Electronics101/SwitchSoftLatch)                           | **MOSFET, BJT**                 test a soft-latching power switching circuit |
| [#204 TemperatureLoggerTypeK](./playground/TemperatureLoggerTypeK)                 | **Sensors, Thermocouple, Arduino**  simple high-temperature monitor using Type K (differential) and LM35 (cold-junction) sensors |
| [#074 TestIR](./playground/TestIR)                                                 | **IR, Arduino**                 test raw IR reception with a TSOP1838-type IR sensor and an Arduino |
| [#267 TheCuttle/ScopeTag](./BoldportClub/TheCuttle/ScopeTag)                       | **Boldport, ATmega, ATmel, Arduino, Digital Pot, MCP42010, Oscilloscope** Get the Boldport Cuttle to write it's name on a Digital Oscilloscope with an MCP42010 digital potentiometer |
| [#281 ThreeStageTransmitter](./Electronics101/FM/ThreeStageTransmitter)            | **FM**                          build an "ugly-style in a can" version of dazaro3's 3-stage FM transmitter circuit |
| [#071 TinyBlink](./playground/TinyBlink)                                           | **Arduino, ATmel**              a simple blink sketch with an ATTINY85-20PU on a breadboard |
| [#137 ToroidJouleThief](./Electronics101/ToroidJouleThief)                         | **Power, RL, Oscillators**      test a "joule thief" circuit based on a ferrite toroid |
| [#135 TouchSwitch/555](./Electronics101/555Timer/TouchSwitch)                      | **555 Timer**                   test a touch switch circuit based on a 555 timer |
| [#228 TransistorCurveTracer](./Electronics101/TransistorCurveTracer)               | **OpAmp, 555 Timer, Oscillators**  simple NPN transistor curve tracer using a Stairstep generator circuit |
| [#083 TransistorTester](./Electronics101/TransistorTester)                         | **Arduino, BJT**                use an Arduino to test NPN and PNP BJTs |
| [#205 TriacDimmer](./Electronics101/TriacDimmer)                                   | **Triac, Thyristor**            investigate the operation of triacs and build the basic dimmaer circuit |
| [#031 Triangle Wave - 555](./Electronics101/555Timer/TriangleWaveGen)              | **555 Timer, Oscillators**      generate a triangle wave with 555 timer and RC integrator |
| [#113 TTLBufferDriver](./Electronics101/TTLBufferDriver)                           | **OpAmp, TTL**                  using an OpAmp as a final buffer stage for TTL or similar circuits |
| [#059 TwoToneDoorbell](./Electronics101/555Timer/TwoToneDoorbell)                  | **555 Timer, Oscillators**      basic two-tone doorbell using a 555 timer oscillator, with n-channel FET for power conservation |
| [#174 UsbNotifier](./Electronics101/UsbNotifier)                                   | **LED, USB**                    tear-down and demo code for some oldUSB Webmail Notifier devices |
| [#145 VariableDutyCycle](./Electronics101/555Timer/VariableDutyCycle)              | **555 Timer, Oscillators**      a 555 oscillator circuit that allows easy manual duty cycle adjustment while minimising the change to frequency |
| [#002 Variable LED brightness with PWM](./playground/VariableLED)                  | **LED, Arduino**                variable resistor is used to control the brightness of an LED with PWM |
| [#276 VariableFrequencyRunwayLEDs](./playground/VariableFrequencyRunwayLEDs)       | **LED, Arduino**                a PWM-controlled variable frequency LED "runway lights" effect using the LM331 and CD4017 |
| [#163 VariableSawtoothGenerator](./Electronics101/VariableSawtoothGenerator)       | **OpAmp, Oscillators**          test a variable-geometry, fixed-amplitude sawtooth wave generator circuit |
| [#125 VoiceLevelIndicatorKit](./Electronics101/VoiceLevelIndicatorKit)             | **LED, Kit**                    build and investigate a commercially available "3-band voice level indicator" kit |
| [#273 VoltageControlledOscillator](./Electronics101/VoltageControlledOscillator)   | **Oscillators, VCO, Varicap**   exploring varicap diodes (KV1471) and their use in frequency tuning of a Colpitts-style voltage-controlled oscillator |
| [#147 VoltageDoublerChargePump](./Electronics101/555Timer/VoltageDoublerChargePump)| **555 Timer, Power**            test a voltage-doubling charge pump circuit based on a 555 timer |
| [#167 VoltageSensorModule](./playground/VoltageSensorModule)                       | **Sensors, Arduino**            test a 25V voltage sensor module with display on a 5110 LCD |
| [#181 VoltmeterModule](./Electronics101/VoltmeterModule)                           | **Sensors**                     test a 3-wire voltmeter module |
| [#097 VolumeControlPowerAmp](./Electronics101/AudioAmps/VolumeControlPowerAmp)     | **OpAmp, Audio**                an LM386 fixed-gain audio power amp with volume control |
| [#164 WatsonLedRing](./Electronics101/WatsonLedRing)                               | **Oscillators**                 test a Watson 3-LED Ring oscillator |
| [#197 WienBridgeAudioToneGenerator](./Electronics101/WienBridgeAudioToneGenerator) | **OpAmp, Oscillators**          fixed-frequency tone generator based on a Wien Bridge Oscillator |
| [#011 X113647Stepper](./playground/X113647Stepper)                                 | **Stepper, Arduino**            using the 28BYJ-48 stepper motor and a X113647 Stepper Motor Driver Board with an Arduino |
| [#265 XYplotter](./playground/XYplotter)                                           | **Arduino, Digital Pot, MCP42010, Oscilloscope** draw pictures on a Digital Oscilloscope using an MCP42010 dual digital potentiometer and an Arduino. Of course, the first thing to try is the classic Christmas Tree |
