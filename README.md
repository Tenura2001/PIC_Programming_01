# PIC_Programming_01
LED blinking using PIC16F887 microcontroller,programming tool is microC pro for pic using microC , use PICkit02

CODING
------------------------

void main() {
     const time = 500;
     SCS_bit=1;
     IRCF0_bit=1;
     TRISD=0;
     PORTD=0;
while(1){
     PORTD.B1=1;
     PORTD.B0=0;
     DELAY_MS(time);
     PORTD.B1=0;
     PORTD.B0=1;
     DELAY_MS(time);
}
}
