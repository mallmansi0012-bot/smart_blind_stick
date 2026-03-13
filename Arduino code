const int trigPin = 9;
const int echoPin = 10;
const int buzzer = 8;
const int motor = 7;

long duration;
int distance;

void setup() {
pinMode(trigPin, OUTPUT);
pinMode(echoPin, INPUT);
pinMode(buzzer, OUTPUT);
pinMode(motor, OUTPUT);
Serial.begin(9600);
}

void loop() {

digitalWrite(trigPin, LOW);
delayMicroseconds(2);

digitalWrite(trigPin, HIGH);
delayMicroseconds(10);
digitalWrite(trigPin, LOW);

duration = pulseIn(echoPin, HIGH);

distance = duration * 0.034 / 2;

if(distance < 50)
{
digitalWrite(buzzer, HIGH);
digitalWrite(motor, HIGH);
}
else
{
digitalWrite(buzzer, LOW);
digitalWrite(motor, LOW);
}

delay(200);
}
