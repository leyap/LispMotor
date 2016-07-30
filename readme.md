# L298x library for arduino

#### provide some useful function make it easy to control car with DC motors use L298x

- leftEn and rightEn must be pwm pin.
- speed range (-255~255)


### Demo
````
#include <LispMotor.h>

//LispMotor(left1=2 left2=4 right1=7 right2=8 leftEn=3 rightEn=5)
LispMotor car (2,4,7,8,3,5);

void setup () {
}

void loop () {
	//car.control(leftSpeed, rightSpeed);
	car.control(50, 50);
	delay (2000);
	car.control(0, 50);
	delay (2000);
}

````
