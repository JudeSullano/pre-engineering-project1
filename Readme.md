



![55FB1B15-FBF0-42C7-A732-C5C21D572363](https://user-images.githubusercontent.com/124808340/218817064-6daed03e-ca46-40d3-8179-91d7232be10c.jpeg)



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


This code reads the button imput by detecting weather or not there is power going through the complete circut
