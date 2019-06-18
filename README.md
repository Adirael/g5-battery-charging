# G5 Battery Charging

The main idea is to swap the two coin cells for a small LiPo (50mAh) with a charging circuit that protects the LiPo, charging it slow. 

To maintain water-proofing you can use magnetic connectors instead of microUSB or similar connectors. Keeping everything enclosed in epoxy waterproofs the rest. 

## Dangers

LiPo cells swell if charged too fast, that added to them being tightly contained (like in this scenario, epoxied in place) can make them explode. This risk is mitigated by charging them slow and using very small batteries.

# Charging circuit 

There's not a lot of space inside a G5 transmitter, to be able to fit everything inside we'll use 50mAh LiPo batteries (10x15x5mm) and SMD components placed in a custom PCB. 

The charging circuit is build around an MCP73831. Using a 20kOhm resistor on the PROG PIN will limit charging current to the smallest setting (50mAh)

## Part list

* MCP73831 in SOT23-5 package
* 470R 0603 package
* 20K 0603 package
* Red LED 0805 package
* 10uF condenser 0805 package
* Pogo pins[4]


[1]: https://thewanderingengineer.com/2016/01/27/simple-lipo-battery-charger-with-the-mcp73831/ 
[2]: https://cdn.sparkfun.com/assets/learn_tutorials/6/9/5/MCP738312.pdf 
[3]: https://ww1.microchip.com/downloads/en/devicedoc/22036a.pdf 
[4]: https://www.aliexpress.com/item/1-par-de-clavijas-magn-ticas-de-resorte-3-pines-de-paso-de-2-3mm-Vertical/32952441488.html?spm=a2g0s.9042311.0.0.274263c0Ow98vr 
