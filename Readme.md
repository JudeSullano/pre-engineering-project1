
https://user-images.githubusercontent.com/124808340/217892202-06d66731-fd41-45bd-9a55-c23a8d4b2d2c.MOV

![BBC3C799-4D06-4946-96E2-28A828861DEF](https://user-images.githubusercontent.com/124808340/217892029-43a5aaa7-52f6-4b75-8eac-2730046572b0.jpeg)


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
