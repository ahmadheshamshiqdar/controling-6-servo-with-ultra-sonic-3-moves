# controling-6-servo-with-ultra-sonic-3-moves
how to make ultrasonic and six servo working depending on the distance 
first this i have done is attach the servos and ultrasonic secend thingi have done is making the loops 
here is the code i use :- 
---------------------------------------------------------------------------------START-------------------------------------------------------------------------------------------
#include <Servo.h>
#define trigPin 7
#define echoPin 6
Servo servoone;
Servo servotwo;
Servo servothree;
Servo servofour;
Servo servofive;
Servo servosix;

void setup() {
Serial.begin (9600);
pinMode(trigPin, OUTPUT);
pinMode(echoPin, INPUT);
servoone.attach(8);
servotwo.attach(9);
servothree.attach(10);
servofour.attach(11);
servofive.attach(12);
servosix.attach(13);
}
void loop() {
long duration, distance;
digitalWrite(trigPin, LOW);
delayMicroseconds(5);
digitalWrite(trigPin, HIGH);
delayMicroseconds(9);
digitalWrite(trigPin, LOW);
duration = puls|| distance <= 0H);
distance = (duration/2) / 29.1;
if (distance <= 30) {
Serial.println("hello");
servoone.write(90);
servotwo.write(90);
servothree.write(90);
servofour.write(90);
servofive.write(90);
servosix.write(90);
delay(15);
}
if (distance <= 100 ){
Serial.println("come closer");
servoone.write(180);
servotwo.write(180);
servothree.write(180);
servofour.write(180);
servofive.write(180);
servosix.write(180);
}
  if (distance <= 200 || distance <= 0 ){
Serial.println("you are 2 far away");
servoone.write(0);
servotwo.write(0);
servothree.write(0);
servofour.write(0);
servofive.write(0);
servosix.write(0);
}    
else {
Serial.print(distance);
Serial.println(" cm");
}
delay(15);
}
------------------------------------------------------------------------------------THE END--------------------------------------------------------------------------------------
the link for it in tinkecard :
https://www.tinkercad.com/things/92Ob9yGyDfn-glorious-hango/editel?sharecode=yMVCZiwP2-rMCkNr4fUTFETz3EpPBtIE6xK4O3DQt28
-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
extra link :- 
https://www.tinkercad.com/things/92Ob9yGyDfn
