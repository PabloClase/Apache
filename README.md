Pasos a seguir configurar Apache2:

-Instalamos apache2 y sus librerías:
 
-Comprobamos el status de apache2
 
-Creamos la carpeta empresazam
 
-Hacemos copia de seguridad del archivo 000-default.conf
 
-Editamos el archivo empresazam.conf y añadimos el DocumentRoot
 
-Aplicamos la cfg del archivo todoempresazam.conf
 
-Restart y status de apache2
 
 

HACER ACCESIBLE A TRAVÉS DE INTERNET LAS SIGUIENTES URL QUE IDENTIFICAN A LA EMPRESA:

-Editamos el archivo /etc/hosts y añadimos la ip con y sin dominio
 
-En el archivo todoempresazam.conf insertamos las líneas ServerName y ServerAlias
 
CONFIGURAR EN EL SERVER LOS TIPOS MIME FORMATO DE VIDEO MP4 EN EL DIRECTORIO VIDEOS:

-Creamos la carpeta videos y añadimos un video

-Editamos de nuevo el archivo todoempresazam.conf y aññadimos la etiqueta Directory con el tipo de formato de video por defecto



CREACIÓN DE SUBDIRECTORIO TODOEMPRESAZAM/DELIMITADO EL DIRECTORIO PRINCIPAL DARÍA ACCESO A CULQUIER USUARIO:

-Creamos la carpeta delimitado en la ruta de la captura:

-Editamos nuevamente el archivo todoempresazam.conf y añadimos la etiqueta Directory con la ruta de la carpeta delimitado y damos acceso a cualquier usuario:

-Creamos el archivo .htacces dentro de la carpeta delimitado

-Creamos la carpeta todoempresazam en la ruta que se muestra en la captura y añadimos el grupo y roles para esa zona

-Creamos la carpeta todoempresazam como se muestra en la captura y creamos el archivo roles:y añadimos los usuarios y grupos para el admin

-Asignamos las pw para root y ness1:

-Creamos las páginas index.html en las siguientes rutas:

-Habilitamos los grupos con el comando a2enmod
 
-Restart y reload de apache2
 
-Accedemos las diferentes zonas desde el navegador
