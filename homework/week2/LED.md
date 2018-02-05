![Blinking LED](CIM-642/homework/week2/images/blinker.jpg)
[Blinking LED](https://youtu.be/tvdK52dYK7k)

int pin1 = 13;
int pin2 = 12;
int pin3 = 8;
int pin4 = 7;


void setup() {
  // put your setup code here, to run once:
  pinMode(pin1, OUTPUT);
  pinMode(pin2, OUTPUT);
  pinMode(pin3, OUTPUT);
  pinMode(pin4, OUTPUT);
}

void loop() {
  // put your main code here, to run repeatedly:
  digitalWrite(pin1, HIGH);
  delay(50);
  digitalWrite(pin1, LOW);
  delay(50);

  digitalWrite(pin2, HIGH);
  delay(50);
  digitalWrite(pin2, LOW);
  delay(50);

  digitalWrite(pin3, HIGH);
  delay(50);
  digitalWrite(pin3, LOW);
  delay(50);

  digitalWrite(pin4, HIGH);
  delay(50);
  digitalWrite(pin4, LOW);
  delay(50);
}
