# sanity test

## setup

Connect 1.8v to pin 4 and gnd to pin 1 of the input connector (J1). Power consumption should be only a few milliampere.

## results

consumption less than 1ma.

# shutdown test

## setup

connect the two pins of the pinheader (J2) together and unpopulate R1. Output voltage should be no higher than input voltage and Power consumption should be only a few microvolts.

## results

works as expected.

# full power test

## setup

Connect 2.2v to pin 4 and gnd to pin 1 of the input connector. Connect a variable resistor between the output (pin 9 of J3) and GND. Start at 1k and adjust the resistor down to about 40R noting the output voltage (pin 9 to pin 1 of J3) at different intervalls.

## results

| current | ripple voltage | output voltage drop |
| ------- | ------------- | ------------------- |
| 1ma     | 150mv         | 0mv                 |
| 33ma    | 200mv         | 0mv                 |
| 66ma    | 200mv         | 0mv                 |
| 100ma   | 190mv         | 0mv                 |
| 110ma   | 150mv         | 50mv                |
| 130ma   | 150mv         | 150mv               |
