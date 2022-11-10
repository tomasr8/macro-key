# Moderately-sized 3D printable USB macro key

- Less than 5€ to make
- Works with any Cherry MX compatible switch
- 59x59mm size
- Support for rubber feet

<p align="middle">
  <img src="./assets/top_view.jpg" width="400" />
  <img src="./assets/side_view.jpg" width="400" />
  <img src="./assets/side_view2.jpg" width="400" />
  <img src="./assets/bottom_view.jpg" width="400" />
</p>

## Bill of materials

- 1x Digispark attiny85 development board (micro USB version) (~2.5€ on aliexpress)
- 1x Cherry MX compatible switch (10 pieces for ~1€ on aliexpress)
- 2x jumper cables
- 2x M3 screws & nuts
- optionally 4x rubber feet (<8mm in diameter)

## Tools

- Soldering iron or electrical tape to connect the jumper wires to the switch legs.
- Arduino IDE to program the board

## Assembly

### Printing

The key consists of two parts - the base and the keycap.
The base can be printed with 0.1mm resolution with supports everywhere.
I printed the keycap with 0.07mm resolution with supports build plate. I also added support blocker for the key cap stem since it's too small for the support to be printed inside it. The keycap should be printed with the highest resolution you can afford to make sure that the stem is printed correctly.

Once the base piece is printed, attach the attiny85 with a pair of M3 screws. Attach two jumper cables to the legs of the switch. I did that by cutting the connectors and soldering the wires to the legs. You could probably also achieve the same thing with a piece of tape. I used an mx black switch in my key (60 cN actuating force) and it works great.

With the connectors attached, place the switch in the bracket in the base piece. Make sure the switch clips into the holes on both sides.
The wires should come out through the hole at the bottom.

After that, you can connect the wires to the tiny. If the wires stick out, you can loop them through the hole to secure them.
I also had to bend the pins on the attiny a little to get the connectors to fit inside.

Once that is done, put the keycap on and you're finished ;)

You might want to sand the keycap depending on the quality of the print and apply some transparent coating for a nice surface finish.

## Programming

http://digistump.com/wiki/digispark/tutorials/connecting

http://digistump.com/wiki/digispark/tutorials/digikeyboard

https://javiervidrua.github.io/blog/jekyll/update/2020/11/06/rubber-ducky-with-digispark-attiny85.html

## Schematic

![](./assets/schematic.png)

https://user-images.githubusercontent.com/8739637/201172834-d55576f6-208d-4fef-8291-895363f8ab84.mp4

