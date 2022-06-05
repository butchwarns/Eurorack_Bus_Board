# Eurorack_Bus_Board

A simple but versatile bus board for modular synthesizers in the Eurorack format.  
It's cheap and easy to build and has many slots for connecting modules with both 10-pin and 16-pin connectors.

![bus board assembled](/pictures/eurorack_bus_board_v010_assembled.jpg?raw=true "bus board assembled")
*Eurorack_Bus_Board (v0.1.0)*

## Motivation

I designed this bus board for use in my own modular synthesizer projects. Thought i'd share the board with other synth builders.
(Gerber files in the repo can be directly uploaded to your pcb manufacturer of choice. Interactive BOM for easy assembly included.)

## A word of caution

**CAUTION:** Use the files in this repository at your own risk!  

If you build this bus board (or anything else involved in powering your modules for that matter), be sure you know how to check for errors in the build before actually hooking it up to power or any precious modules! Don't fry a module with a connector wrongly soldered upside down!  

I will do my best to test everything, but the occasional bug might still find its way into the project files. Don't hesitate to report found bugs or share ideas on how to improve the board.

## Project status

The *main* branch of this repository holds the current tested version of the board. All potentially breaking changes will be done on the *develop* branch and the build will be tested before merging. Images in this README do not necessarily show the most recent version of the board, though all images will have version numbers in their title.  

## Tech/framework used

- KiCad

## Features

- Connection for 20 modules (split evenly between 10-pin and 16-pin headers)
- Designed for use with standard +12V, -12V, +5V power.  
- Follows the Doepfer Eurorack standard including the internal busses for CV and gate.  
- Three LEDs indicate the rails being powered.
- 1.5A max current per rail (can probably take a bit more with appropriate wiring, but better be on the safe side)

## Installation

M3 screws and PCB spacers can be used to mount the board to the back of a case.  
Regular 6.3mm flat connectors are used for connecting to the power suppply.

## How to use?

Connect some modules and power the case?  

You can connect power to either side of the board or even chain multiple bus boards in series. (Do not exceed maximum current!)

## How to build?

Upload the *.zip* in the `gerber_files/` folder to your PCB manufacturer's website to order.

An interactive HTML BOM is available in the `bom/` folder. Just open it in a browser and tick off sourced/placed components.  
Also shows where on the board components should be placed.  

**HINT:** Use good quality solder/flux and clean the board thoroughly after soldering!  
Flux residue (especially from low quality solder) may form slightly conductive bridges between power rails, which are very noticeable when there's 40 of them in parallel. I recommend isopropyl alcohol (isopropanol) for cleaning circuit boards.

## Component availability/choices

No unobtainium in this project. All components should be easily sourced.  

Any 1.8mm LEDs will do fine. You might need to tweak the current limiting resistors for equal brightness, which can easily be done on a breadboard.  

Capacitor values are absolutely uncritical as well. The board would probably work with all R,C and LED omitted, although this was neither intended nor tested.

## Contact

Any questions?   

🡢 contact[at]butchwarns.de

## License

*(TODO: Find appropriate open-hardware license!)*

> Until otherwise stated here, the project is default licensed as proprietary.

Build as many of these boards as you want for personal use, but please make it obvious if your build has modified the project files in any way to avoid confusion!  

My name and any logo of mine that might me present on the board design are copyrighted and are not free to use.

Feel free to share the images in the `pictures/` folder of this repository with correct attribution or a link to the project.  

Copr. 2021, Butch Warns
