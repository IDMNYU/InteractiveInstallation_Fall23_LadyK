## Circuit Basics

![Image of a simple circuit](http://www.faqs.org/docs/electric/DC/00032.png)

#### Electricity

Electricity is the movement of electrons. Electrons create a charge, which we can harness to do the work of turning things on and powering things.

* Voltage - Voltage is synonymous with pressure. Voltage changes around the circuit, based on the components in the circuit. There is a difference in voltage between two points. You can think of voltage as how much the water valve is turned (strength). Or how high a water fall is. It is measured in Volts

* Current - The rate at which the charge is flowing through your circuit, the moving of electrons from the negative source on your battery, through your circuit to the positive source on your battery.  Current is measured in Amps and is represented by the letter I.

* Resistance - Resistance is what limits the flow of current in your circuit. Think of this as your thumb over a garden hose. It is measured in Ohms and is represented by the letter R.

### Ohm's Law

Georgia Ohm, A Bavarian Scientist who stuided electricity, found that there is a direct proportionality between the potential difference (voltage) applied across a conductor. This is known as [Ohm's Law](https://en.wikipedia.org/wiki/Ohm%27s_law)

Combining the above elements of voltage, current and resistance, he developed the formula below:

#### **V = I * R**

* V = Voltage (volts)
* I = Current (amps)
* R = Resistance (ohms)



### Okay that's great. But What Size Resistor Do I Need?

Check out the datasheet for your LED’s. This can be found on your vendor’s website. On that datasheet, look for the value listed under forward voltage. You might see something like, “typical forward voltage of 2.2, maximum 2.5, and a forward current of 20mA.“ 

Now say you have a 9volt battery and are working with 1 LED. Subtract 2.5volts (the amount the LED needs) from the 9volts and we get 6.5 volts. We need a resistor that will take 6.5 volts from the circuit (leaving 2.5 for the LED). In any given circuit, the total voltage around the path of the circuit is zero

Remember, current is the same throughout your simple circuit. The amount of current going into any point in a circuit is also the same amount of current coming out of that component. If we want a maximum of 20 mA to flow through the LED, the same amount of current needs will be flowing through the resistor.

Converting all the units to volts, amps and ohms, sot that 20MA should be written as 0.02 amps:

		V = 6.5 (the potential drop across the resistor)
		I = 0.02 (the current flowing through the resistor)

We want to know R, the resistance. So, we use the version of Ohm’s Law that puts R on the left side:

		R = V/I

Plug in our values:

		R = 6.5/0.02

And we get:

		325 Ohms

325 Ohms is a standard size, so we move to the next closest standard size of 330 ohms.

[LED Calculator](http://led.linear1.org/1led.wiz)

[LED Calculator for Series and Parallel Circuits](http://led.linear1.org/led.wiz)

### Series Circuit

![Series Circuit](http://www.siyavula.com/gr7-9-websites/technology/gr7/Tech_English_LB_Grade7_term3_1-web-resources/image/Tech2_gr7_ch3_fig5_opt.jpeg)

![Series Circuit](https://www.msnucleus.org/membership/html/k-6/as/technology/4/images/series.gif)

When energy flows from one component to the next, the components are in series. When resistors are in series, the voltage drops across each resistor. Therefore, the total resistance is equal to the sum of all the resistors. **Resistors divide voltage when in series.**

R(total) = R1 + R2 + R3 ....

![Series Circuit](https://www.ibiblio.org/kuphaldt/electricCircuits/DC/00098.png)

### Parallel Circuits

![parallel circuits](https://www.cdli.ca/courses/ep/predesign/t03/02knowledge-skills/images/activity10/pirtorial-parallel.jpg)

![Parallel circuit](https://www.teachengineering.org/collection/cub_/lessons/cub_images/cub_electricity_lesson06_activity1_figure1.jpg)

When energy flows through all the components at the same time, the components are in parallel. For resistors in parallel, the voltage across them is equal, but the current is divided between them. The divided current across the parallel resistors is equal to the total current. **Resistors divide amerage when in parallel.**

1/R(total) = 1/R1 + 1/R2 + 1/R3 ...

![Image of parallel circuit of resistors](http://sub.allaboutcircuits.com/images/00083.png)


#### Further Reading and Reference:



**[SparkFun Tutorial on Electricity](https://learn.sparkfun.com/tutorials/voltage-current-resistance-and-ohms-law)**

**[Tom Igoe site](http://www.tigoe.com/pcomp/code/circuits/understanding-electricity/)**

**[ITP Tutorial](https://itp.nyu.edu/physcomp/lessons/electronics/electricity-the-basics/)**

**[All About Circuits](http://www.allaboutcircuits.com/textbook/direct-current/chpt-1/voltage-current/)**

**[Make Electronics by Charles Platt](http://www.amazon.com/Make-Electronics-Learning-Through-Discovery/dp/1680450263/ref=sr_1_1?ie=UTF8&qid=1459296290&sr=8-1&keywords=make+electronics)**

**[Manga Guide to Electricity by Kazuhiro Fujitaki](http://www.amazon.com/Manga-Guide-Electricity-Kazuhiro-Fujitaki/dp/1593271972/ref=sr_1_1?s=books&ie=UTF8&qid=1459296360&sr=1-1&keywords=manga+guide+to+electricity)**