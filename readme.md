# Grundlæggende forståelse i Arduino og C-programmering

## Opgave: Tænd og sluk en LED med en trykknap 

>1. Opsætning af Arduino: 
>    * Tilslut din Arduino til computeren via USB. 
>    * Åbn Arduino IDE (Integrated Development Environment). 
>    *  Vælg den korrekte Arduino-model og port under “Værktøjer” > “Board” og “Port”. 
>2. Hardwareopsætning:
>    * Forbind en LED til pin 13 (anvend en modstand for at undgå skade på LED’en).
>    * Forbind en trykknap til en anden pin (f.eks. pin 2). 
>3. Variabler og kontrolstrukturer: 
>    * Definér en variabel for LED-pinden: int ledPin = 13; 
>    * Definér en variabel for trykknap-pinden: int buttonPin = 2; 
>4. Kode: 
>~~~c
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
>~~~
> 5. Koden tænder LED’en, når trykknappen er trykket ned, og slukker den, når knappen er frigivet. 
>6. Upload:
>    * Klik på “Upload” i Arduino IDE for at overføre koden til din Arduino. 
>7. Test: 
>    * Tryk på knappen og se, hvordan LED’en reagerer! 

Husk at udforske Arduino-referencen for flere funktioner og muligheder. God fornøjelse med programmering! 🚀 

 ## Opgave 2: Du skal nu udvide opgaven og udfordre dig yderligere: 
 
### Variabel lysstyrke: 

> Tilføj en potentiometer (drejeknap) til en analog indgang (f.eks. A0). 
>
>* Brug potentiometeret til at justere lysstyrken på LED’en. Jo højere værdi fra potentiometeret, desto lysere LED’en skal være. 
>
>Flere LED’er: 
>
>* Tilføj flere LED’er til forskellige digitale pins. 
>
>Brug knappen til at skifte mellem LED’erne  
>
>* (f.eks. første tryk tænder LED 1, andet tryk tænder LED 2 osv.). 
>
### Tidsbaseret kontrol: 
>
> Brug millis()-funktionen til at tænde/slukke LED’en med en bestemt >tidsforsinkelse. 
>
>* F.eks. tænd LED’en i 5 sekunder, når knappen trykkes, og sluk derefter. 
>
> Blinkende LED: 
>
>* Implementer en blinkende effekt på LED’en. 
>
>* Du kan bruge delay() eller millis() til at styre blinkhastigheden. 
>
### Flere knapper: 

>* Tilføj flere trykknapper og tildel forskellige handlinger til hver knap (f.eks. tænd/sluk LED’er, skift farve osv.). 
>
### Brug af biblioteker: 
>* Du kan bruge Arduino-biblioteker (f.eks. Servo, LiquidCrystal, Wire osv.) til at løse opgaven. 
>* Du kan udforsk mulighederne for at tilføje mere kompleks funktionalitet. 