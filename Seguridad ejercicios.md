
Hash:

Un hash en ciber seguridad se refiere a una funcion matematica que toma u n conjuntos de datos y produce una cadena de caracteres alfanumericcos de longitud fija que representa de manera unica los datos originales

Integridad de datos
contraseñas seguras
almacenamiento seguro
verificacion de descargas
firma digital

ripemd
Torbellino


La tecnica HMac


estenografía

gpg4wink
veracrypt


gnuPG en linux


Payload:son los datos que deseamos transportar
encoding desnsity: El porcentaje de bits, muestras u otros elemntos de señal seran modificados para codificado el payload
LSB(least significant Bit):El bit menos significativo
cover:El objeto(archivo digitado)en el cual se va incrustrar u ocultar un mensaje o archivo. También llamado carrier
Stego-image: Es la imagen que se forma con la imagen original
stego-key: Es la clave que se utiliza cuando se oculta el mensaje 
stegalisis: El arte de descubrir datos ocultos en objetos cover


Pura:No requiere el intercambio de un cifrado como un stego-key
Clave secreta: La clave secreta(stego se intercambia antes de la comunicacion
De clave publica: Se utiliza una clave publica y una clave privada para una comunicacion segura

Tecnicas estenograficas

Enmascaramiento:marcas de agua
Algoritmos de la compresion de datos:funciones matematicas
Metodos de sustitucion: Alterando el bit menos significativo

estegoanalisis

stegdetect
stegosuite
Ilook Investigator
EnCase



gpg -c [documento] (cifrar)
		-d (decifrar)

gpg --gen-key
gpg -a --export [usuario] > [nombre del archivo].asc

gpg -kv
gpg --import [documento]

gpg -a -r [destinatario] -r [enviador] --encrypt