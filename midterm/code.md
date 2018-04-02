const int flexpin1 = 4; //pinky
int led1 = 3;

const int flexpin2 = 3; //ring
int led2 = 5;

const int flexpin3 = 2; //middle
int led3 = 6;

const int flexpin4 = 1; //index
int led4 = 9;

const int flexpin5 = 0; //thumb
int led5 = 11;

void setup() {
  
  Serial.begin(9600);

}

void loop() {

  int flexposition1;

  flexposition1 = analogRead(flexpin1);
  analogWrite(led1, flexposition1);
  Serial.print("sensor: ");
  Serial.print(flexposition1);

  delay(20);

  int flexposition2;

  flexposition2 = analogRead(flexpin2);
  analogWrite(led2, flexposition2);
  Serial.print("sensor: ");
  Serial.print(flexposition2);

  delay(20);

  int flexposition3;

  flexposition3 = analogRead(flexpin3);
  analogWrite(led3, flexposition3);
  Serial.print("sensor: ");
  Serial.print(flexposition3);

  delay(20);

  int flexposition4;

  flexposition4 = analogRead(flexpin4);
  analogWrite(led4, flexposition4);
  Serial.print("sensor: ");
  Serial.print(flexposition4);

  delay(20);

  int flexposition5;

  flexposition5 = analogRead(flexpin5);
  analogWrite(led5, flexposition5);
  Serial.print("sensor: ");
  Serial.print(flexposition5);

  delay(20);

}