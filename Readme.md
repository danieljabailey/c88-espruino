#C88 Emulator for Espruino

##Usage
Simply download the c88-espruino.js to the espruino

##Wiring

I haven't made a proper schematic yet, until then there is this list of definitions mostly takend from the JS code:

```
LED_MATRIX_MOSI = B15; //(DIN)
LED_MATRIX_SCK  = B13;
LED_MATRIC_CS   = B14;

DATA_SWITCHES   = [A15, A14, A13, A10, A9, A8, C11, C10];
ADDR_SWITCHES   = [C9, C8, C7];
WRITE_BUTTON    = C6;
USER_SWITCH     = C5;
RUN_SWITCH      = C4;
PC_VIEW_BUTTON  = A1;
MEM_VIEW_BUTTON = A0;
REG_VIEW_BUTTON = C3;
SPEED_SWITCH    = C2;
STEP_BUTTON     = C15;
RESET_BUTTON    = C12;
```

The code doesn't set up any pull-ups and so all switches and buttons need external pull-ups (or all pins wired on DPST switches) or you could add in the code to do it, I did this in a hurry and so didn't add it.

##Copyright, etc:

Copyright Daniel Bailey and Nick Moriarty 2015

This software is distributed under the GNU Lesser General Public Licence

Details here: http://www.gnu.org/licenses/lgpl.html


Nick's original JS simulator repo is here: https://github.com/aquila12/c88-js
