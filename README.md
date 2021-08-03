# Rear-Wheeled-Bobbycar
For the rear wheeled version of the Bobbycar you do not need to know much about electronics or software. I will just give you a few links for information and my CAD data for the chassis.

## Software

### Motor Controller
Emanuel Feru wrote a FOC Firmware for the Hoverboard Controllers. This is the one you should flash, but you can also take the original from Niklas Fauth.

Links:
- The used Software for Inverters, took out of Hoverboards https://github.com/EmanuelFeru/hoverboard-firmware-hack-FOC
- The original Software for Inverters, took out of Hoverboards https://github.com/NiklasFauth/hoverboard-firmware-hack

My preferred IDE for the Hoverboard Software is Visual Studio Code with PlatformIO. You have to restart your PC a few times during the installation, that helped me as things did not want to appear as supposed. You can set up the config.h as you like and you can even make changes to the main.c or other files to implement new features. Keep in mind that you should not delete safety features.
Be careful in Torque Mode if you want to get more speed. The MC Software has a bug at high speed. You can drive very fast in field weakening, but then, if you let go the throttle too fast, it brakes really hard. That will not happen if you set the field weakening current in config.h to a normal value like 5-6 Ampere. IF YOU SET IT HIGHER, TELL EVERYONE WHO DRIVES ABOUT THAT ISSUE. 

ST-Link:
You should use a ST-Link V2 for programming the Motor Controllers and the Main Controller.
- ST-Link V2 https://www.ebay.de/sch/i.html?_nkw=st-link+v2&_sop=12
- Virtual COM Port Drivers https://www.st.com/en/development-tools/stsw-stm32102.html

STM32 ST-Link Utility:
From factory the Hoverboard Motorcontrollers are locked, so you have to unlock them by using the STM32 ST-Link Utility and a Flash Device called ST-Link V2. To use the ST-Link you have to install the Virtual COM Port Drivers.
- STM32 ST-Link Utility https://www.st.com/en/development-tools/stsw-link004.html
- How To Unlock https://github.com/EmanuelFeru/hoverboard-firmware-hack-FOC/wiki/How-to-Unlock-MCU-Flash

## Electronics
Take apart an old XBox360 Controller and get those two potentiometers out of it. Solder them to the Controller like larsm did: https://larsm.org/allrad-e-bobby-car/

DO NOT solder 15V to the potentiometers. They will kill your Motorcontroller.

## Mechanics
The provided CAD Model is built in Autodesk Inventor, but there you can also find a step export later.


### Frame
The Frame is built from 6mm and 21mm Plywood (Sperrholz), the kind with long fibres, not pressboard/particle board (Pressspan). Plywood is much more rigid.
There are dxf-files under "Mechanics" for lasercutting. Cutting by Hand is also possible, therefor you need an A3 printer and a jigsaw.
After cutting, 12mm parts are glued together out of 6mm pieces, then everything is pushed together and tightend by screws.
If you want your wood to last longer in the rain i recommend to paint it.

### Steering
You really should change the front tires, the original ones have no grip and understeer as hell. Also they have no bearings, which lets them overheat because you are not a kid anymore. I took the ones from Decathlon with 175mm in diameter. Those with a 8mm Screw and a piece of steel pipe (8mm Inner, 10mm Outer) as an adapter to the original wheel carrier work far better.
If the lowest part of your steering gets loose and the "thread" in the bobbycar wears out, you can screw a small piece of wood to the inside.



# Drift Tires
Yeah, you read it right, i built drift tires for this. Fortunately a pipe in Germany named "Kanalgrundrohr" has the right size for this and is made out of PVC. A slice of this can be glued to printed PLA parts, which are mounted to the hoverboard motors using an TPU adaptor. This has been built, but not been tested yet. I am confident that it will work.



# Formula-Student-Mini
Maybe we can establish a formula competition which is about small, extremely low cost and high powered vehicles. At my University we set up some rules. Some are for safety, some are to harmonize cars and some are for fun.
- Rules https://github.com/Kowitzki/Four-Wheel-Bobbycar/blob/main/Formula%20Student%20Mini%20-%20Rules%20V1.pdf

We have a Telegram Group for the Bobbycars, get in there, maybe someone will help you: https://t.me/FormulaStudentMini



# Other Instructions for Bobbycars
- https://larsm.org/allrad-e-bobby-car/
- https://figch.de/index.php?nav=bobbycar



# Safety
- Do not charge unattended
- Do not delete safety features
- Do not drive on public streets
- Use a deadman switch for driving
- Think about what you want to do



# Beer
If you like my effort, i would appreciate if you get me a beer ;)
www.paypal.me/kowitzki/2.00
