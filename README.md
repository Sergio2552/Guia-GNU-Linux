# Navegar en GNU/Linux




# Manejo de archivos




# Package Management 

## Debian / Ubuntu

Para la administracion de paquetes dentro de las distribuciones basadas en Debian/Ubuntu usamos 

### Instalar paquetes.
	
Para instalar paquetes por medio del **sistema administrador de paquetes** tenemos 2 opciones:


		$ apt install <package-name>
		or
		$ apt-get install <package-name>

		
Aunque ambos comandos hacen la misma funcion **apt** (Advanced Package Tool) es la mejora del comando **apt-get**, aunque el segundo no esta descontinuado por lo que es seguro usarlo. En caso de duda usar **apt** que es mas amigable al usuario.

---

Para instalar paquetes *.deb*  es por medio del comando **dpkg** (Debian Package) con la siguiente sintaxis:

		$ dpkg -i PACKAGE_NAME.deb
		
Por medio de **dpkg** (que es un administrador de paquetes) podemos instalar los archivos con extension *.deb* (comparable al *.exe* de Microsoft Windows) estos archivos hay que resaltar que son para distribuciones basadas en Debian o en Ubuntu.


### Desinstalar paquetes.

Para desinstalar paquetes mediante el **sistema administrador de paquetes** tenemos 2 opciones:

		$ apt remove PACKAGE_NAME
		or 
		$ apt-get remove PAKAGE_NAME

La opcion `remove` nos sirve para eliminar el paquete/binario, pero si deseamos que tambien se eliminen los archivos de configuracion remanentes reemplazar la opcion `remove` por `purge`.

___

Para desinstalar paquetes *.deb*  por medio del comando **dpkg** (Debian Package) con la siguiente sintaxis:
		
		$ dpkg -r PACKAGE_NAME
		
Para tambien eliminar los archivos de configuracion remanentes cambiar la opcion `-r` por `-P`.


### Actualizar paquetes.

Para actualizar paquetes mediante el **sistema administrador de paquetes** podemos actualizar todos los paquetes (con actualizaciones disponibles) con los comandos:

		$ apt update && apt upgrade
		
La opcion `update` hace que el sistema actualice su lista de paquetes disponibles y actualizaciones, la opcion `upgrade` descarga y ejecuta la actualizacion de los paquetes.

Para actualizar solo un determinado paquete usamos:

		$ apt --only-upgrade install PACKAGE_NAME
	
Si nosotros previamente ejecutamos el comando `apt update` entonces como ya tenemos actualizados las listas de nuestros paquetes simplemente con el siguiente comando podemos actualizar el paquete que necesitemos:

		$ apt install PACKAGE_NAME
		

___


Para actualizar paquetes *.deb*  por medio del comando **dpkg** (Debian Package) con la siguiente sintaxis:

		$


## RedHat / Fedora / Centos


### Instalar paquetes.
Para instalar paquetes por medio del **sistema administrador de paquetes**, con el comando **dnf** (Dandified YUM):

		$ dnf install <package-name>

El comando **dnf** es la actualizacion y mejora del comando **yum** (Yellowdog Updater,Modified), por lo cual para administrar paquetes en distribuciones basadas en RedHat es muy preferible usar **dnf** aunque todavia hay compatibilidad con **yum** (no usar en distribuciones mas actualizadas por razones de documentacion, rendimiento, etc.).

___

Para instalar paquetes *.rpm* se utiliza el comando **rpm** (RedHat Package Manager) con la siguiente sintaxis:

		$ rpm -i PACKAGE_NAME.rpm
		
Por medio de **rpm** (que es un administrador de paquetes) podemos instalar los archivos con extension *.rpm* comparable al *.exe* de Microsoft Windows) estos archivos hay que resaltar que son para distribuciones basadas en Redhat y derivados.

	
### Desinstalar paquetes.



### Actualizar paquetes.


## SUSE / openSUSE

### Instalar paquetes.

Para instalar paquetes por medio del **sistema administrador de paquetes**, con el comando **zypper** (Dandified YUM):

		$ zypper install <package-name>
		or
		$ zypper in <package-name>   #in=install

El comando **zypper** es la interface para el sistema de administracion de librerias *ZYpp*, este comando es muy versatil y completo.

___

Para instalar paquetes *.rpm* tenemos 2 opciones usar el comando **zypper** o el comando **rpm**:

		$ zypper in PACKAGE_NAME.rpm
		or
		$ rpm -i PACKAGE_NAME.rpm



### Desinstalar paquetes.

Para desinstalar paquetes mediante el **sistema administrador de paquetes** usamos el siguiente comando:

		$ zypper remove PACKAGE_NAME
		or 
		$ zypper re PAKAGE_NAME



___



### Actualizar paquetes.

Para actualizar paquetes mediante el **sistema administrador de paquetes** podemos actualizar todos los paquetes (con actualizaciones disponibles) con los comandos, previamente a estos tenemos que actualizar los repositorios con el comando `zypper refresh`:

		$ zypper update
		or
		$ zypper up  #up=update

Si queremos actualizar un paquete en especifico usamos el siguiente comando:

		$ zypper update PACKAGE_NAME
		or
		$ zypper up PACKAGE_NAME
		
## Arch

### Instalar paquetes.
Para instalar paquetes por medio del **sistema administrador de paquetes**, con el comando **pacman** (Package Manager):

		$ pacman -S <package-name>
		or
		$ pacman -U PACKAGE_NAME.pkg.tar.xz 


Con el comando **pacman** podemos instalar paquetes desde los repositorios oficiales o desde un archivo local.

___

Para instalar paquetes desde el *Arch User Repository* se utiliza el comando **yay**, estos paquetes son mantenidos por la comunidad:

		$ yay -S <package-name>

Anteriormente la interface para los repositorios de la comunidad era **yaourt** el cual ya no recibe soporte, hay que resaltar que tanto **yay** y **yaourt** no son las unicas herramientas para los repositorios de la comunidad ya que hay mas variedad disponible (aunque con menos popularidad).

### Desinstalar paquetes.



### Actualizar paquetes.



# Administrar servicios




# Comandos











#### Fuentes

Debian package management - https://www.debian.org/doc/manuals/debian-reference/ch02.en.html


SUSE / openSUSE package managemnet - https://en.opensuse.org/images/3/30/Zypper-cheat-sheet-2.pdf




Gracias a los desarrolladores de Ghostwriter por su programa que facilito la elaboracion de esta guia.

https://docs.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax

https://github.github.com/gfm/

https://guides.github.com/features/mastering-markdown/
