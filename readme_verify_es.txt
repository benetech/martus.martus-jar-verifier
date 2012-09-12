Martus(tm) Software readme_verify_es.txt
----------------------------------------

Benetech contin�a mejorando el programa Martus. Visite el sitio http://www.martus.org para obtener la versi�n, m�s reciente y siga 
las instrucciones en la p�gina Web para verificar la copia descargada 
usando el programa SHA-1 sum. 

En el futuro, Benetech puede distribuir una versi�n actualizada 
del archivo martus.jar. No debe confiar la autenticidad de ning�n 
archivo martus.jar que reciba separadamente a menos que lo haya 
verificado usando el procedimiento que sigue. No conf�e en ning�n otro 
m�todo de verificaci�n que se le haya dado separadamente. 

Use s�lo el programa de verificaci�n incluido en un CD de instalaci�n 
de Martus. Las instrucciones asumen que el programa de verificaci�n 
esta ubicado en la carpeta �Verify� en el CD de instalaci�n de Martus. 
Posiblemente sea necesario alterar estas instrucciones si es que ha 
copiado el programa de verificaci�n a un disquete o a su disco duro. 


* En Windows: 

Abra una ventana de MS-DOS y escriba las tres l�neas siguientes, 
sustituyendo la letra �d� por la de su unidad de CD-ROM y la ubicaci�n 
del archivo .jar que esta verificando: 

d: 
cd \verify 
ves d:\ubicacion-De-Archivo\martus.jar 

o, desde el men� Inicio, escoja Ejecutar y luego escriba: 

d:\verify\ves d:\ubicacion-De-Archivo\martus.jar 

(donde la letra d es la letra asignada a su unidad de CD-ROM y ubicacion-De-Archivo es la ubicaci�n del archivo .jar que est� verificando). 

Si ve el mensaje �Martus JAR verified.� (Martus JAR verificado) significa 
que el archivo .jar es leg�timo. 


* En Mac OS: 

Coloque el archivo .jar nuevo en la carpeta Martus existente en su disco 
duro y luego ejecute el programa verificador: 

Abra el programa Terminal y escriba los siguientes comandos: 

cd /Volumes 
ls 
cd Martus (oprima la tecla Tab para auto completar el nombre de la carpeta) 
cd verify 
java -cp . JarVerifier /Library/Java/Martus/martus.jar 

Si ve el mensaje �Martus JAR verified.� (Martus JAR verificado) significa 
que el archivo .jar file es leg�timo. 

* En Linux: 

Coloque el archivo .jar file en la carpeta existente ~/.Martus/ y ejecute 
el programa verificador. Las siguientes l�neas pueden ser copiadas a 
una ventana bash o sh (aunque quiz� sea necesario ser el usuario 
'root' para poder ejecutar el comando mount): 

mount=/mnt/cdrom 
[ -d $mount ] || mount=/cdrom # para Debian y etc 
[ -d $mount/[vV]erify ] || mount -r $mount 
cd $mount/[vV]erify && java JarVerifier ~/.Martus/martus.jar 

Si ve el mensaje �Martus JAR verified.� (Martus JAR verificado) significa 
que el archivo .jar es leg�timo. 

Si ve el mensaje �bash: java: No such file or directory� (bash: java: No 
existe ese archivo o carpeta) entonces es necesario agregar la carpeta 
'bin' de Java a su variable de entorno PATH. Consulte con el primer paso 
del procedimiento de instalaci�n de Linux. 

Si ve el mensaje �Error loading class JarVerifier: Bad major version 
number� (Error al cargar la clase JarVerifier: Versi�n mayor 
incorrecta) entonces necesita instalar una versi�n de Java m�s reciente 
y/o poner la versi�n m�s reciente de Java en la variable PATH de su 
entorno. Consulte con el primer paso del procedimiento de instalaci�n 
de Linux. 


