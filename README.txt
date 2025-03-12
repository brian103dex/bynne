3 lü potansiye rgb
int K=2; 
int Y=3;
int M=4;
void setup() {
	pinMode(K, OUTPUT);  
	pinMode(Y, OUTPUT);  
	pinMode(M, OUTPUT);  
}

void loop()
{
  int Kpot = analogRead(A0); 
  int Kled = map(Kpot, 0, 1023, 0, 255);
  int Ypot = analogRead(A1); 
  int Yled = map(Ypot, 0, 1023, 0, 255);
  int Mpot = analogRead(A2); 
  int Mled = map(Mpot, 0, 1023, 0, 255);    
 analogWrite(2, Kled); 
 analogWrite(3, Yled); 
 analogWrite(4, Mled);  
}