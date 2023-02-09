int buttonPin = 13;
int buttonState = 0;

void setup() {
Serial.begin(9600);
pinMode(buttonPin, INPUT);
}

void loop() {
delay(500);
buttonState = digitalRead(buttonPin);
if (buttonState == HIGH)
  {
  Serial.println("Button Pressed");
  }
  else
  {
  Serial.println("Waiting");
    }
}
