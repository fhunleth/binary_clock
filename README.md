# Binary Clock

This is a companion site to Chapter 6 of [Build a Binary Clock with Elixir and Nerves](https://pragprog.com/titles/thnerves/build-a-binary-clock-with-elixir-and-nerves/).

Bruce and I wrote a book in 2021 and found out that buying the hardware was
hard. Depending on when you read this, that hopefully has changed. This
repository was our attempt to take the easiest to buy LED controller at the time
(TM1620) and build a PCB that runs the clock. (If we're going to make a PCB, we
might as well go all the way and make it a proper Raspberry Pi hat.)

*Boards are not available for sale yet. When they are details will be posted here*

This repository contains all of the materials for creating the Binary Clock that
we talk about in Chapter 6. It may differ from the text as we find ways to
improve it.

Project directories:

* `datasheets` - Datasheets for the TM1620
* `hw` - Schematics and layout for the PCB. These can be loaded into
  [EasyEDA](https://easyeda.com/) which is a free PCB design tool. EasyEDA
  supports exports to other PCB design tools.
* `notebooks` - Notebooks that can be loaded into [Nerves
  Livebook](https://github.com/livebook-dev/nerves_livebook) for experimenting
  with the clock in the Livebook UI.

## FAQ

1. What if I can't find a Raspberry Pi?

(Insert scream here.)

It seems like if you place an order at one of the online stores selling Pis that
you eventually will get one. The [rpilocator.com](https://rpilocator.com/)
website may help.

## Notes for exporting from EasyEDA

(For Frank) EasyEDA lets you store projects on their website, but it's nice to
track copies here as well.

1. Right click on the `binary_clock2` project in the project side bar. Click
   "Manage Project->Download".
2. Unzip the downloaded file and copy the `.json` files to the `hw` directory.
3. Export the schematic as a PDF and copy to the `hw` directory.
