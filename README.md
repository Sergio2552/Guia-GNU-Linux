# Navegar en GNU/Linux




# Manejo de archivos




# Package Management 

## Debian / Ubuntu

### Instalar paquetes.
	
Para instalar paquetes por medio del **sistema administrador de paquetes** tenemos 2 opciones.

		$ apt install <package-name>
		or
		$ apt-get install <package-name>
		
Aunque ambos comandos hacen la misma funcion **apt** (Advanced Package Tool) es la mejora del comando **apt-get**, aunque el segundo no esta descontinuado por lo que es seguro usarlo. En caso de duda usar **apt** que es mas amigable al usuario.

---

Para instalar paquetes *.deb*  es por medio del comando **dpkg** (Debian Package) con la siguiente sintaxis:

		$ dpkg -i PACKAGE_NAME.deb
		
Por medio de **dpkg** (que es un administrador de paquetes) podemos instalar los archivos con extension *.deb* (comparable al *.exe* de Microsoft Windows) estos archivos hay que resaltar que son para distribuciones basadas en Debian o en Ubuntu.


### Desinstalar paquetes.



### Actualizar paquetes.





## RedHat / Fedora / Centos


### Instalar paquetes.
Para instalar paquetes por medio del **sistema administrador de paquetes**, con el comando **dnf** (Dandified YUM).

		$ dnf install <package-name>

El comando **dnf** es la actualizacion y mejora del comando **yum** (Yellowdog Updater,Modified), por lo cual para administrar paquetes en distribuciones basadas en RedHat es muy preferible usar **dnf** aunque todavia hay compatibilidad con **yum** (no usar en distribuciones mas actualizadas por razones de documentacion, rendimiento, etc.).

___

Para instalar paquetes *.rpm* se utiliza el comando **rpm** (RedHat Package Manager) con la siguiente sintaxis:

		$ rpm -i PACKAGE_NAME.rpm
		
Por medio de **rpm** (que es un administrador de paquetes) podemos instalar los archivos con extension *.rpm* comparable al *.exe* de Microsoft Windows) estos archivos hay que resaltar que son para distribuciones basadas en Redhat y derivados.

	
### Desinstalar paquetes.



### Actualizar paquetes.


## openSUSE
Para instalar paquetes por medio del **sistema administrador de paquetes**, con el comando **zypper** (Dandified YUM).

		$ zypper install <package-name>
		or
		$ zypper in <package-name>   #in=install

El comando **zypper** es la interface para el sistema de administracion de librerias *ZYpp*, este comando un muy versatil y completo		

### Instalar paquetes.


### Desinstalar paquetes.



### Actualizar paquetes.


## Arch

### Instalar paquetes.
Para instalar paquetes por medio del **sistema administrador de paquetes**, con el comando **pacman** (Package Manager).

		$ pacman -S <package-name>
		or
		$ pacman -U PACKAGE_NAME.pkg.tar.xz 


Con el comando **pacman** podemos instalar paquetes desde los repositorios oficiales o desde un archivo local.

___

Para instalar paquetes desde el *Arch User Repository* se utiliza el comando **yay**, estos paquetes son mantenidos por la comunidad.

		$ yay -S <package-name>

Anteriormente la interface para los repositorios de la comunidad era **yaourt** el cual ya no recibe soporte, hay que resaltar que tanto **yay** y **yaourt** no son las unicas herramientas para los repositorios de la comunidad ya que hay mas variedad disponible (aunque con menos popularidad)

### Desinstalar paquetes.



### Actualizar paquetes.



# Administrar servicios




# Comandos












Gracias a los desarrolladores de Ghostwriter por su programa que facilito la elaboracion de esta guia.
