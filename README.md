# A smart raised garden bed Irrigation-Solution
A smart raised garden bed irrigation-control with home assistant and esphome. This is my first own project - so please be kind :)

## What is this?
I´ve created a smart raised garden bed irrigation-control to use with home assistant. I use different parts for this. The watering-solution is a cheap "plug-and -play-pump-in-a-water-tank"-solution from a discounter. Once it is connected to power the pump pumps water for 1-minute every 12 hours. I use an wifi-controlled socket to power it on and off. After powering it on it pumps water for 1 minute and the 12-hour timer starts. Since i want the pump to work more often then every 12 hours, i power the plug off after the pumps finishes its 1-minute-work and power it on every 60 minutes (could be any time you wish). So i do have control over the amount of water that will go to the raised garden bed.

If the tank runs out of water, the bottom-water-level-sensor will notice that and control my zigbee-controlled water-outled to fill the tank up. The upper water-level-sensor will notice that the tank is full and close the water-outlet.

## What do i need?
- a dumb "plug-and-play-pump-in-a-water-tank"-solution (~ 40 Euros - [Link](https://www.ebay.de/itm/204000996870?chn=ps&norover=1&mkevt=1&mkrid=707-134425-41852-0&mkcid=2&itemid=204000996870&targetid=1269408113723&device=c&mktype=pla&googleloc=9043753&poi=&campaignid=10203814920&mkgroupid=119187118461&rlsatarget=pla-1269408113723&abcId=1145991&merchantid=7364532&gclid=CjwKCAjwh-CVBhB8EiwAjFEPGfIB4Qsaj-7PJZuJnQFHyd9olH7OTvuo5YQFUwloD3XU3n5Sv0UOYRoCK90QAvD_BwE))
- a zigbee-controlled water-outlet (~ 40 Euros - [Link](https://www.amazon.de/gp/product/B08M9RWQP6/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1))
- an wifi- or zigbee-controlled smart-plug (~ 10 Euros - could be any smart plug home assistant can control)
- ESP32-Board (~ 10 Euros - [Link](https://www.amazon.de/dp/B071P98VTG/ref=twister_B07Z6CSD9K?_encoding=UTF8&psc=1))
- Breadboard (~ 4 Euros - [Link](https://www.amazon.de/gp/product/B07KKJSFM1/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&th=1))
- "Housing" for the ESP32 (~ 15 Euros for 10 - [Link](https://www.amazon.de/gp/product/B09D3YNZSL/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1))
- USB-Power-Plug and USB-Cable (took one i had laying around here)
- 2 x Water-Level-Sensors (~ 15 Euros for 4 - [Link](https://www.amazon.de/gp/product/B09B1KQV7B/ref=ppx_yo_dt_b_asin_title_o07_s00?ie=UTF8&psc=1))
- 2 x 10k-Resistor (~ 9 Euros for a whole box of resistors [Link](https://www.amazon.de/gp/product/B07Q87JZ9G/ref=ppx_yo_dt_b_search_asin_title?ie=UTF8&psc=1)

## Hardware-Setup
![image](https://user-images.githubusercontent.com/29648553/175833356-20f04f1c-4e77-4b29-9e7c-c16920f21035.png)

## Sofware-Setup

### ESPHOME
See [ESPhome-Yaml-Code](https://github.com/guevara777/smart_raised_garden_bed_irrigation/blob/main/esphome_code.yaml)

### Automation in Home Assistant
