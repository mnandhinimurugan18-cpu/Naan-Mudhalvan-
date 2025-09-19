# Naan-Mudhalvan-
This Arduino program controls an LED using a push button. The LED is connected to pin 13 and the button to pin 7. In setup(), pin 13 is set as OUTPUT and pin 7 as INPUT. In loop(), the button state is read. If pressed (HIGH), the LED turns ON; if not pressed (LOW), the LED turns OFF. It shows simple digital input-output control.
int ledPin = 13;    
int buttonPin = 7;  
int buttonState = 0;

void setup() {
  pinMode(ledPin, OUTPUT);     
  pinMode(buttonPin, INPUT);  
}

void loop() {
  buttonState = digitalRead(buttonPin); 

  if (buttonState == HIGH) {
    digitalWrite(ledPin, HIGH);
  } else {
    digitalWrite(ledPin, LOW);   LED OFF
  }
}






