# Portable-Charger
Portable charger using active rectifier circuit

This circuit is made with the interest in the generation of power
and management of the same we present a Portable Cell
Phone Charger that can be used any where .Also this device
is convenient to be handled when anyone is on outdoor trips
.This device is both practical and convenient. It is obvious
that a device that could charge cell phone batteries just by
the use of human harvesting energy is a very appealing and
valuable product . My main aim here is to replace the diodes
which have a cut off voltage of 0.7 V with transistors which
is cheaper more mechanical sensitivity and lower threshold
voltage. Here I will just present the simulations of a manual
simple charger replace with MOS in my final simulation .

There are 2 parts of the circuit 1) The rectification and 2)
The voltage regulation. The circuit consists of a AC input
source of already stepped down voltage as the step down
transformer in Spice can’t be modelled. The Transformer
turns ratio should be calculated via the given below formula
equation Np/Ns equals to Ep/Es where the Ns is the number if turns in the primary coil and the Ns is the number of
turns in the secondary coil . The Ep is the voltage across the
primary node and the Es is the voltage across the secondary
node and the capacitance values to reduce the ripple must be
calculated by the C=1/2xfxVripple , where C is the capacitor filter and the V ripple is the ripple we want to attain or
desire . The output then rectified via a full wave bridge rectifier as the sub circuit where I have used Mosfet as switches
instead of diodes .In this final report circuit I have not been
able to implement a LM7805 as the spice net list was not
included in the ESIM software, instead I used a DC 5 V to
just simulate the circuit. Actually the output of the rectifier
will be passed through a LM7805 voltage regulator whose
output is always 5V. LM7805 is a voltage regulator which
will regulate any input voltage across it input to 5 voltage
but up to a certain limit so we need to absolutely sure that
there is not much voltage drop across the input components
of the LM7805. A Zener of 5V voltage rating will be used to
protect the LM7805 and the output from getting distorted.
Isolation diode is used in between rectifier and voltage regulator.
