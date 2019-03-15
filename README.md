int brilloB;
int brilloG;
int brilloR;
int blue= 5;
int green= 6;
int red= 3;


void setup() {
Serial.begin(9600);
pinMode(blue, OUTPUT);
pinMode(green, OUTPUT);
pinMode(red, OUTPUT);
}

void loop() {
valorB = analogRead(A1);
valorG = analogRead(A0);
valorR = analogRead(A2);
brilloB = map(valorB, 0, 1023, 0, 255);
brilloG = map(valorG, 0, 1023, 0, 255);
brilloB = map(valorB, 0, 1023, 0, 255);
analogWrite(blue, brilloB);
analogWrite(green, brilloG);
analogWrite(red, brilloR);

}
