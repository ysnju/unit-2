```C
// C++ code
//
void setup()
{
  pinMode(LED_BUILTIN, OUTPUT);
  Serial.begin(9600);
  
  bool bit0 = true;
bool bit1 = true;
bool bit2 = true;
int dec = 0;
//Trace this program
for(int k=0; k<2; k+=1){
    bit2 =!bit2;
    for(int j=0; j<2; j+=1){
  bit1 = !bit1; //not operation
  for(int i=0; i<2; i+=1){
      bit0 = !bit0;
      Serial.print(dec);
      Serial.print(bit2);
      Serial.print(",");
      Serial.print(bit1);
      Serial.print(",");
      Serial.println(bit0);
      dec ++;
      }
    
}


}
}

void loop()
{
  digitalWrite(LED_BUILTIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  digitalWrite(LED_BUILTIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
  

}
```
