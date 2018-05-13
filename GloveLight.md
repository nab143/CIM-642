# Glove Light

## Project Description:
## This smart glove uses three buttons to control three different modes of light. The first button turns a white light on and off. The second button turns a blue light on and off. The third button turns a UV light on and off.

## This smart glove was inspired by the Iron Man hand. It was originally intended to convert sign language into different LED modes. Using flex sensors and LEDs, hand gestures were meant to control light brightness, and color. However, the fragile flex sensors broke in the process of the build. As the next step, the glove light will be updated to work with the flex sensors and multiple bright LED rings. 

## Equipment:
## (1) Arduino Uno
## (1) Breadboard - Self-Adhesive
## (3) Push Buttons
## (10) White LEDs
## (8) Blue LEDs
## (6) UV LEDs
## Jumper Wires
## (3) 10kΩ Resistors
## (3) 220Ω Resistors
## Glove
## Black Fabric
## Sewing Kit/Velcro Tape
## Electrical Tape

## How its Made:

## The glove uses three push buttons (placed on horizontally on the wrist of the glove), to read each press and tell the LED to turn on or off. 

## Step 1: Give common ground and electricity (5V) from the Arduino to the breadboard. 

## Step 2: Connect the push buttons to the breadboard with 10k resistors. 

## Step 3: Give pin connections to each of the push buttons. I used:

## Step 4: Connect each type (3) of LEDs (White/Blue/UV) to the breadboard with 220 resistors.

## Step 5: Give pin connections to the each type of LED.

## Step 6: Connect each type of LED to a push button on the breadboard.

## Step 7: Connect Arduino to PC and upload the code. 

## Code:

## const int buttonPin1 = 2;     // Button One
## const int ledPin1 =  8;      // White LED

## const int buttonPin2 = 4;     // Button Two
## const int ledPin2 =  7;      // Blue LED

## const int buttonPin3 = 76;     // Button Three
## const int ledPin3 =  4;      // UV LED

## int buttonState1 = 0;         // variable for reading the Button One status
## int buttonState2 = 0;         // variable for reading the Button Two status
## int buttonState3 = 0;         // variable for reading the Button Three status

## void setup() {
##  // initialize the White LED pin as an output:
##  pinMode(ledPin1, OUTPUT);
##  // initialize the Button One pin as an input:
##  pinMode(buttonPin1, INPUT);

##  // initialize the Blue LED pin as an output:
##  pinMode(ledPin2, OUTPUT);
##  // initialize the Button Two pin as an input:
##  pinMode(buttonPin2, INPUT);

##  // initialize the UV LED pin as an output:
##  pinMode(ledPin3, OUTPUT);
##  // initialize the Button Three pin as an input:
##  pinMode(buttonPin3, INPUT);
## }

## void loop() {
##  // read the state of Button One value:
##  buttonState1 = digitalRead(buttonPin1);

##  // read the state of Button Two value:
##  buttonState2 = digitalRead(buttonPin2);

##  // read the state of Button Three value:
##  buttonState3 = digitalRead(buttonPin3);

##  // check if Button One is pressed
##  if (buttonState1 == HIGH) {
##    // turn White LED on:
##    digitalWrite(ledPin1, HIGH);
##  } else {
##    // turn White LED off:
##    digitalWrite(ledPin1, LOW);
##  }

##  // check if Button Two is pressed
##  if (buttonState2 == HIGH) {
##    // turn Blue LED on:
##    digitalWrite(ledPin2, HIGH);
##  } else {
##    // turn Blue LED off:
##    digitalWrite(ledPin2, LOW);
##  }

##  // check if Button Three is pressed
##  if (buttonState3 == HIGH) {
##    // turn UV LED on:
##    digitalWrite(ledPin3, HIGH);
##  } else {
##    // turn UV LED off:
##    digitalWrite(ledPin3, LOW);
##  }
  
## }