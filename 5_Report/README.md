# REPORT

## ABSTRACT:
   #### In this project a door sensor is connected to 1 bit of port b.
   #### Port c is connected to an led in which it can sense whether the door ids opened or not.
   #### Here an voltage regulator is kept for displaying the voltage to the door i.e switch and to the led.
   #### Input and output were kept for the efficient output. 
   #### And here atmega 328 microcontroller is used for the door sensor.
   
## INTRODUCTION 
#### In this project there will be a switch which acts as a door and an led which is connected in port c.
#### when the door is opened the led will glow sensing that the door has been opened.

## OBJECTIVE
#### The main objective of this project is to sense the door.
#### To sense whether it is open or closed.
#### This is actually indicated by an led which is connected.

## FEATURES
#### The door sensor to sense the door.
#### Also with an LED.

## CODE
#### #include <avr/io.h>
#### int main(void)
#### {
#### DDRB=DDRB&0b11111101;//fd
#### DDRC=DDRC|0b01000000;//40
#### while(1)
#### {
#### if(PINB & 0b00000010)//02
#### PORTC=PORTC|0b01000000;//40
#### else
#### PORTC=PORTC&0b10111111;//bf
#### }
#### return 0;
#### }

## SIMULATION
![door sensor 1](https://user-images.githubusercontent.com/101242023/164491888-535a8bc9-7c20-46e9-9d8b-5943575886ce.png)

## OUTPUT
![Door sensor output](https://user-images.githubusercontent.com/101242023/164493770-64ffdce7-805c-4adb-b0a9-e1a1e7fc2fd9.png)




