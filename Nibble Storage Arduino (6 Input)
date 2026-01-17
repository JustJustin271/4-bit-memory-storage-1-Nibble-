const int btn1 = 2; //ONES
const int btn2 = 3; //TWOS
const int btn3 = 4; //FOURS
const int btn4 = 5; //EIGHTS

const int ePin = 7; //ENABLE
const int rPin = 8; //RESET

const int ledPin1 = 10; //ONES
const int ledPin2 = 11; //TWOS
const int ledPin3 = 12; //FOURS
const int ledPin4 = 13; //EIGHTS

bool latch1 = LOW; //Start off and low
bool latch2 = LOW; //Start off and low
bool latch4 = LOW; //Start off and low
bool latch8 = LOW; //Start off and low

void setup() {
  //I'd be defining those pins there bru
  pinMode(btn1, INPUT_PULLUP);
  pinMode(btn2, INPUT_PULLUP);
  pinMode(btn3, INPUT_PULLUP);
  pinMode(btn4, INPUT_PULLUP);

  pinMode(ePin, INPUT_PULLUP);
  pinMode(rPin, INPUT_PULLUP);

  pinMode(ledPin1, OUTPUT);
  pinMode(ledPin2, OUTPUT);
  pinMode(ledPin3, OUTPUT);
  pinMode(ledPin4, OUTPUT);
}

void loop() {

  if (digitalRead(ePin) == LOW) {

    delay(20);
    
      if (digitalRead(btn1) == LOW) {
      latch1 = HIGH;
    }
      if (digitalRead(btn2) == LOW) {
      latch2 = HIGH;
    }
      if (digitalRead(btn3) == LOW) {
      latch4 = HIGH;
    }
      if (digitalRead(btn4) == LOW) {
       latch8 = HIGH;
    }
    delay(50);
  }

    if(digitalRead(rPin) == LOW) {
      latch1 = LOW;
      latch2 = LOW;
      latch4 = LOW;
      latch8 = LOW;
      delay(100); //GIVE THAT SHIIIII TIME TO COOOOKK 
    }

  delay(50);

  //Make 'em lights turn on :D 
  
  digitalWrite(ledPin1, latch1);
  digitalWrite(ledPin2, latch2);
  digitalWrite(ledPin3, latch4);
  digitalWrite(ledPin4, latch8);
  
}
