The 2020 Ford Ranger engine bay has limited space, and the battery I am interested in installing (a [LiFePO<sub>4</sub>](https://en.wikipedia.org/wiki/Lithium_iron_phosphate_battery) battery) does not fare well in a hot engine bay.

## Battery selection

I have selected a [12V 100Ah smart LiFePO<sub>4</sub> battery](https://www.renogy.com/12v-100ah-smart-lithium-iron-phosphate-battery/) from Renogy as it can be easily hacked with Python or Arduino running on something like a Raspberry Pi Pico for monitoring and control via [RS-485](https://en.wikipedia.org/wiki/RS-485) [Modbus](https://en.wikipedia.org/wiki/Modbus) protocol. This is important to me as I do not wish to embrace any particular ecosystem that will lock me down.

## Installation location

Two options remain:

- install battery in cab of truck
- install battery in bed

The first option comes with some inherent safety concerns that in my mind are too severe to consider an in-cab installation.

This leaves me with one option: Install the battery somewhere in the truck bed.

## Background and motivation

My Ranger is equipped with a Retrax XR Pro tonneau cover that provides ample protection from the elements and nosy thieves. It can be locked in virtually any position which has proven to be very helpful.

The slight downside of the XR Pro is that it rolls back into a canister that takes up a fair bit of space in the front of the bed. This has impacted several other design decisions and led to some needed customizations of other parts of the in-bed storage.

However, this presents a unique opportunity: place the battery under the canister for the tonneau cover, avoiding the drain pipes for the canister itself. The battery will have ample protection in this location and even if loose, would not be able to cause extended kinetic damage during a rollover or similar accident.

## Protecting the battery

I have iterated on how to best protect the battery from custom steel battery boxes to commercially available battery holders. I have settled on a battery box from Noco that works well for the LiFePO<sub>4</sub> battery I am using.

The battery box still needs to be anchored to the bed of the truck.

### Optimal conditions

The safe operating temperature ranges of the Renogy battery are as follows:

| Condition                      | Range    |
| ------------------------------ | -------- |
| Standard operating temperature | 25℃±5℃   |
| Storage temperature            | -25~65℃  |
| Charge temperature             | 0~55°C   |
| Discharge temperature          | -20~60°C |

I have measured the temperature in the bed of the truck with a thermometer over the past few weeks, and the temperatures rarely reach over 105°F (40.5°C). The tonneau cover and the tent I have mounted above the bed tend to give the bed quite a bit of shade, and this is promising as far as optimal conditions go.

## Pulling cable to the aux battery

The aux battery needs clean power. I have a set of well-shielded 2 AWG welding cables made out of oxygen free copper strands. These should be more than capable of transferring energy from the starter battery to the front of the bed.