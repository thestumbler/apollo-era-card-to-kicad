# Apollo-Era-Card-RevEng

See the accompanying Hackaday writeup about this schematic project:

[https://hackaday.com/2024/11/25/apollo-era-pcb-reverse-engineering-to-kicad](
https://hackaday.com/2024/11/25/apollo-era-pcb-reverse-engineering-to-kicad)


This repo documents additional explorations into the reverse engineering
effort of an Apollo-era printed circuit board assemly that Skyhawkson
obtained earlier this year. See his project at the [original
repo](https://github.com/Skyhawkson/Apollo-Era-Card-RevEng/tree/main).

Note: I planned to submit this as a pull request to Skyhawkson's
repository. But I ran into trouble with git and spaces in filenames, a
problem I haven't seen before. 


### Best Guess

This is an interface board for reading sensors such as strain gauges. 
It features a precision voltage source to excite the bridge. It also 
has a differential amplifier to scale up the sensor voltage and
proportionally drive an output load. The output stage has an enable pin,
suggesting that multiple card outputs may be multiplexed into one analog
to digital circuit card. That makes sense, since scanning through a
bunch of sensors over and over again makes sense in the context of
running through test sequences.

If there are any updates based on comments from Hackaday readers or
anyone here in GitHub, or just random new insights, I will update the
repository as necessary.

### Schematic

Schematic [(PDF)](eda-logical/logical-sch.pdf)

![](eda-logical/logical-sch.png)



### Original Readme

Reverse Engineering an Apollo-Era Circuit Card

https://github.com/Skyhawkson/Apollo-Era-Card-RevEng/tree/main

[Writeup on hackaday.io](https://hackaday.io/project/194704-reverse-engineering-an-apollo-era-circuit-card)

![Board Front Cropped](board-images/board-front-cropped.jpg)



