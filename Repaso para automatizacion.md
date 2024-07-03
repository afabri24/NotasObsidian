

variables

int nombreDeVariable=Valor;

constantes

#define nombreConstante valor

que es setup y loop

setup: es un codigo que solo se va ejecutar una vez

loop: Es un codigo que se va ejecutar varias veces


Cuales serian los componentes de salida

luces led
pantalla lcd
bocina
motores

Cuales serian los componentes de entrada

Sensores 
Boton

Cual es la diferencia de ser pin digital a un pin analogico

Digital: Solamente tiene 2 valores: 0 y 1

Analogico: va desde 0 a un valor de 1023

Cuales pines son los unicos que van a tener high o low o entrada y salida?

digital
Por que los analogicos solamente son de entrada


como mandarias una señal digital al pin 3

int pin=3;

pinMode(pin,OUTPUT);

digitalwrite(pin,HIGH);

como leerias una señal digital al pin 5

int pin=3;

pinMode(pin,INPUT);

valorPin=digitalread(pin);


como leerias una señal analogica de A0:

analogread(A0);

como mandarias una señal analogica de A1;

analogwrite(A1,125);


Que hace este codigo;


void setup(){
	pinMode(2,OUTPUT); //configura el pin para que sea de salida
	pinMode(3,OUTPUT);

}

void loop(){
	digitalwrite(2,HIGH);
	delay(1000);
	digitalwrite(2,LOW);
	digitalwrite(3,HIGH);
	delay(1000);
	digitalwrite(3,LOW);
	
}