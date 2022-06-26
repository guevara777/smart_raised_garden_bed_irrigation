# smart_raised_garden_bed_irrigation
A smart raised garden bed irrigation-control with home assistant and esphome

## What is this?
I´ve created a smart raised garden bed irrigation-control to use with home assistant. I use different parts for this. The watering-solution is a cheap "plug-and -play-pump-in-a-water-tank"-solution from a discounter. Once it is connected to power the pump pumps water for 1-minute every 12 hours. I use an wifi-controlled socket to power it on and off. After powering it on it pumps water for 1 minute and the 12-hour timer starts. Since i want the pump to work more often then every 12 hours, i power the plug off after the pumps finishes its 1-minute-work and power it on every 60 minutes (could be any time you wish). So i do have control over the amount of water that will go to the raised garden bed.

If the tank runs out of water, the bottom-water-level-sensor will notice that and control my zigbee-controlled water-outled to fill the tank up. The upper water-level-sensor will notice that the tank is full and close the water-outlet.

## What do i need?
- a dumb "plug-and-play-pump-in-a-water-tank"-solution (~ 40 Euros - [Link](https://www.ebay.de/itm/204000996870?chn=ps&norover=1&mkevt=1&mkrid=707-134425-41852-0&mkcid=2&itemid=204000996870&targetid=1269408113723&device=c&mktype=pla&googleloc=9043753&poi=&campaignid=10203814920&mkgroupid=119187118461&rlsatarget=pla-1269408113723&abcId=1145991&merchantid=7364532&gclid=CjwKCAjwh-CVBhB8EiwAjFEPGfIB4Qsaj-7PJZuJnQFHyd9olH7OTvuo5YQFUwloD3XU3n5Sv0UOYRoCK90QAvD_BwE))
