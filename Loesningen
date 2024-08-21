# Løsning på opgaven

>~~~c
>int ledPin = 13;
>int buttonPin = 2;
>
>void setup() 
>{
>  pinMode(ledPin, OUTPUT); // Sæt LED-pinden som output 
>
>  pinMode(buttonPin, INPUT_PULLUP); // Sæt trykknap-pinden som input med pull-up modstand
>} 
>
>void loop() 
>{ 
>    int buttonState = digitalRead(buttonPin); // Læs trykknap-tilstanden  
>
>    if (buttonState == LOW) // Hvis knappen er trykket ned 
>    { 
>        digitalWrite(ledPin, HIGH); // Tænd LED'en 
>    } 
>    else 
>    { 
>        digitalWrite(ledPin, LOW); // Sluk LED'en 
>    } 
>} 
