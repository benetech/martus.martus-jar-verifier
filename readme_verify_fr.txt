Logiciel Martus� readme_verify_fr.txt
-------------------------------------

Benetech am�liore constamment l�application Martus. Allez sur http://www.martus.org pour r�cup�rer la derni�re version et suivez les instructions sur le site web pour valider le logiciel t�l�charg� � l�aide du programme  SHA-1 sum .

A l�avenir, Benetech choisira peut-�tre de distribuer une version mise � jour du fichier martus.jar. Ne faites confiance � aucun fichier martus.jar qui vous serait livr� s�par�ment, tant que vous n�avez pas v�rifi� son authenticit� � l�aide de la proc�dure ci-apr�s. Ne faites confiance � aucune autre proc�dure de v�rification qui vous aurait �t� fournie par d�autres moyens. 

N�utilisez que le programme de v�rification fourni sur un CD Martus authentique. Les instructions ci-dessous assument que le programme de v�rification se situe dans le r�pertoire "Verify" (v�rifier) d�un CD Martus. Si vous avez plac� le programme de v�rification sur une disquette ou sur le disque dur, il vous faudra modifier ces instructions en cons�quence.


* Sous Windows :

Ouvrez une fen�tre d�invite MS-DOS et saisissez les trois lignes suivantes, en rempla�ant la lettre "d" par celle de votre propre CD-ROM ainsi que le chemin d�acc�s au fichier .jar que vous v�rifiez :

d:
cd\verify
ven d:\chemin-fichier\martus.jar

OU BIEN, � partir du menu D�marrer, choisissez Ex�cuter, puis saisissez :

d:\verify\ven  d:\chemin-fichier\martus.jar  

(d �tant la lettre correspondant � votre CD-ROM et chemin-fichier �tant le chemin menant au fichier .jar que vous v�rifiez).	

Si la ligne "Martus JAR verified" (Martus JAR v�rifi�) s�affiche � l��cran, le fichier .jar est l�gitime.


* Sous Mac OS :

Placez le nouveau fichier .jar dans le dossier Martus existant sur votre disque dur, puis ex�cutez le programme de v�rification : 

Ouvrez la fen�tre d�application du Terminal, puis saisissez les commandes suivantes :

cd  /Volumes
ls
cd  Martus (puis tapez la touche Tab pour remplir automatiquement le nom du dossier)
cd  verify
java  -cp  .  JarVerifier  /Library/Java/Martus/martus.jar

Si la ligne "Martus JAR verified" (Martus JAR v�rifi�) s�affiche � l��cran, le fichier .jar est l�gitime.


* Sous Linux :

Placez le nouveau fichier .jar dans le r�pertoire ~/.Martus/ existant, puis ex�cutez le programme de v�rification. Le code suivant peut �tre coll� dans un bash ou sh shell (bien qu�il vous faille peut-�tre vous trouver � la racine ("root") pour ex�cuter la commande mount):

  mount=/mnt/cdrom
  [ -d $mount ] || mount=/cdrom		# for Debian and etc
  [ -d $mount/[vV]erify ] || mount -r $mount	
  cd $mount/[vV]erify && java JarVerifier ~/.Martus/martus.jar

Si la ligne "Martus JAR verified" (Martus JAR v�rifi�) s�affiche � l��cran, le fichier .jar est l�gitime.  

Si vous lisez "bash: java: No such file or directory" (bash: java: Fichier ou R�pertoire inexistant) vous devrez alors ajouter le r�pertoire 'bin' de java � votre CHEMIN D�ACCES (PATH). Voir �tape 1 de la proc�dure d�installation Linux.   

Si vous lisez "Error loading class JarVerifier : Bad major version number" (Erreur de chargement class JarVerifier : Mauvais num�ro de version principale) vous devrez alors installer une version plus r�cente de java, et/ou placer la derni�re version de java plus en amont de votre chemin (PATH). Voir �tape 1 de la proc�dure d�installation Linux.
