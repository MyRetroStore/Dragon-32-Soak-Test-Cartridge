# Dragon 32 Soak Test Cartridge

From the description on [WorldOfDragon](https://archive.worldofdragon.org/index.php?title=Dragon_32_Soak_Test)

_A cartridge designed to test the Dragon 32 hardware in a loop.
The ROM program will change a pattern on screen and lit a green led on the cartridge if tests are passing, and freeze the machine and lit a red led if any test fails.
The cartridge will not work on a Dragon 64 or a Dragon 200 as it performs a ROM checksum and later models will make the checksum test fail._

There is not much documentation on the Soak Test Cartridge for the Dragon 32 computer. 

After finding a photo of the PCB on WorldOfDragon I decided to reverse engineer the PCB 
and with the help of the community on the forums as well as a Dragon 32 Facebook group, I've managed to re-create the schematic and a replica PCB.

## Folders
Hardware - Schematic, PCB layout and Gerbers created with [KiCad](https://www.kicad.org/) 7.0.10

ROM - Binary file from worldofdragon.org

Photos - Photos of the orignal and replica PCB as well as screenshots of the cartridge in action. 


![PCB](https://github.com/MyRetroStore/Dragon-32-Soak-Test-Cartridge/blob/main/Photos/Dragon%2032%20Soak%20Test%20Cardridge%20Replica%20TOP.jpg)

![Inserted](https://github.com/MyRetroStore/Dragon-32-Soak-Test-Cartridge/blob/main/Photos/Dragon%2032%20Soak%20Test%20Cardridge%20Replica%20Insert1.jpg)

![Screenshot](https://github.com/MyRetroStore/Dragon-32-Soak-Test-Cartridge/blob/main/Photos/Dragon%2032%20Soak%20Test%20Cardridge%20Replica%20Screen1.jpg)

![Screenshot](https://github.com/MyRetroStore/Dragon-32-Soak-Test-Cartridge/blob/main/Photos/Dragon%2032%20Soak%20Test%20Cardridge%20Replica%20Screen2.jpg)


## BOM

| Reference  | Component                           |
| ---------- | ----------------------------------- |
| C1	       | 10u Electrolytic Capacitor          |
| C2,C3      | 10n Ceramic Capacitor               |
| D1	       | Red 5mm LED                         |
| D2	       | Green 5mm LED                       |
| DC1-4	     | 100n Ceramic Capacitor (Decoupling) |
| IC1	       | 74LS04                              |
| IC2	       | LM555                               |
| IC3	       | EPROM 27C64                         |
| IC4	       | 74LS10                              |
| R1-2, R5-8 | 3k3 Resistor 0.25W                  |
| R3         | 100k Resistor 0.25W                 |
| R4	       | 1k Resistor 0.25W                   |
| TR1,TR2    | BC237 Transistor                    |

I've tested the PCB in my Dragon 32 and it seems to work as expected, however I do not take any responsibility if you are building this and there is damage done to your Dragon 32 due to incorrect assembly or it doesn't work as expected. 

While this should be as close as possible a 100% replica to the orignal PCB there could be some error (Though hopefully not. Let me know if you find any) 



