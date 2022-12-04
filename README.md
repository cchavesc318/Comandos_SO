## Comandos SistemasOperativos-Caroline Chaves

Comandos Vistos en Clase

|Num|Comandos Linux|Descripcion|Ejemplo|
|-|--------|-------------|------------|
|1|`cat`|para crear o imprimir archivos|`cat> archivo.txt`|
|2|`mv`|para mover documentos u otros|`mv archivoamover lugaramover`|
|3|`ls`|para mostrar lo que haya dentro de un directorio carpeta etc|`ls home/`|
|4|`tail`|para ver las ultimas lineas de determinado archivo|`tail /var/log/blah`|
|5|`mkdir`|para crear directorios o subdirectorios|`mkdir archivoacrear`|
|6|`sudo`|sede permisos para ejecutar codigos|`sudo apt-install ejemplo`|
|7|`apt-install`|para instalar paquetes (aplicaciones)|`apt install google-chrome`|
|8|`cp`|es para copiar archivos|`cp archivo.txt /lugar/donde/se/va/a/mover`|
|9|`*.blah`|este es para buscar archivos con esa terminacion|`cp *.log /lugar`|
|10|`su`|ingresar a la root|`su`|
|11|`rm`|para eliminar datos,archivos,carpetas y asi sin importar si estan llenos o no|`rm datos`|
|12|`-R`|es para hacer acciones de manera recursiva|`rm -R datos`|
|13|`adduser`|esto es para crear un nuevo usuario|`adduser nombreusuario`|
|14|`passwd`|es para cambiar la contraseña|`passwd usuarioacambiarcontra`|
|15|`dpkg -i, -e, -c`|para administrar paquetes a través de su instalación, eliminación y compilación|`dpkg -i loquequerramosinstalar`|
|16|`alias`|para crear shortcuts de acciones|`alias shortcut="sudo apt update && sudo apt upgrade"`|
|17|`ps`|para hacer un seguimiento de tu memoria y uso de la CPU|`ps`|
|18|`-aux'|para crear un nuevo archivo con determinado comando|`ps -aux`|
|19|`grep -i (imprimir nombre), -f(buscar en un doc), -w(busca palabra completa), -o(muestra linea)`|para buscar archivos con una determinada palabra|`grep palabraclave`|
|20|`ssh`|es para la comunicación encriptada y segura entre dos sistemas sobre una red no segura.|`ssh nuestramaquina`|
|21|`scp`|copia archivos o directorios entre un sistema local y un sistema remoto, o entre dos sistemas remotos.|`scp archivo maquina/ysu/ubicacion`|
|22|`exit`|para salir de la terminal|`exit`|
|23|`pwd`|para saber la ruta en la que estamos actualmente|`pwd`|
|24|`nano`|editar el texto en la consola|`nano archivo`|
|25|`ls -a`|para mostrar los archivos ocultos|`ls -a`|
|26|`clear`|para limpiar la consola|`clear`|
|27|`rm -Rf`|para borrar de manera forzada|`rm -Rf`|
|28|`cd ..`|lo direcciona a /home|`cd ..`|
|29|`kill`|para matar procesos o terminarlos|`kill numbredelproceso`|
|30|`ip a`|para ver la direccion ip|`ip a`|
|31|`apt update`|para actualizar el sistema|`sudo apt update`|
|32|`apt upgrade`|para mejorar el sistema|`sudo apt upgrade`|
|33|`history`|para ver el historial de comando usados|`history`|
|34|`whoami`|para ver el usuario que estemos usando|`whoami`|
|35|`top`|para mostrar el estado de los procesos de la maquina|`top`|
|36|`htop`|para el estado de otro sistema de la maquina|`sumo apt install htop`|
|37|`ps -auclx`|terminal no interactiva, imprime en pantalla el estado de los procesos|`sudo ps -auclx`|
|38|`pstree`|para mostrar los procesos en forma de arbol|`sudo pstree`|
|39|`sudo mkdir /blah/ram_disk`|para crear una particion en la memoria ram|`sudo mount -t tmpfs -o size=1024m new_ram_disk /mnt/ram_disk`|
|40|`du`|para ver tamaño de un archivo|`sudo du`|
|41|`stat`|para modificar fechas|`sudo stat archivo`|
|42|`file`|para saber el formato del archivo|`sudo file archivo`|
|43|`chmod`|para cambiar el acceso de algun directorio|`chmod archivo /home`|
|44|`chown`|para cambiar el propietario|`chown archio nuevopropietario`|
|45|`df -h`|para saber el espacio del disco usado|`df -h`|
|46|`mount`|para el montaje de archivos como usb|`mount usb`|
|47|`gnome-disk-utility`|para mostrar las particiones|`sudo gnome-disk-utility`|
|48|`vim`|para editar un archivo|vim archivo|
|49|`touch`|para crear un archivo|touch archivo|

Comandos usados en el Proyecto

|*|Comandos|Descripcion|Uso|
|-|--|--------|-------|
|*|`sudo raspi-config`|para configurar el rasp|`sudo raspi-config`|
|*|`ifconfig`|para saber informacion|`ifconfig`|
|*|`sudo apt install proftpd`|para instalar la app|`sudo apt install proftp`|
|*|`sudo nano /ect/proftpd/proftpd.config`|nos abre el archivo de instalación donde se asigna el nombre y los permisos del servidor|`sudo nano /ect/proftpd/proftpd.config`|
|*|`sudo service proftpd reload`|para recargar el ftp|`sudo service proftpd reload`|
|*|`sudo service proftpd status`|nos permite ver que el servidor se configuró correctamente y se encuentra activo|`sudo service proftpd status`|
|*|`sudo useradd -m -s /bin/bash FTPUSER`|creamos un usuario, el cual será como un usuario administrador|`sudo useradd -m -s /bin/bash FTPUSER`|
|*|`sudo passwd FTPUSER`|para cambiarle la contraseña al usuario|`sudo passwd FTPUSER`|
|*|`sudo cp /etc/proftpd/proftpd.conf /etc/proftpd/proftpd.conf.bak`|para hacer una copia del archivo de instalación, esto es únicamente una medida de respaldo en caso de que sea necesario|`sudo cp /etc/proftpd/proftpd.conf /etc/proftpd/proftpd.conf.bak`|
|*|`sudo openssl genrsa -out /etc/ssl/private/proftpd.key 4096`|para crear un key|`sudo openssl genrsa -out /etc/ssl/private/proftpd.key 4096`|
|*|`sudo nano /etc/proftpd/proftpd.conf`|para agregar el certificado a la configuración, editando nuevamente el archivo de configuración|`sudo nano /etc/proftpd/proftpd.conf`|
|*|`sudo chmod 0600 /etc/ssl/private/proftpd.key`|para asegurse que tanto el key como el certificado no sean modificados y estén seguros|`sudo chmod 0600 /etc/ssl/private/proftpd.key`|
|*|`sudo chmod 0600 /etc/ssl/certs/proftpd.crt`|para asegurse que tanto el key como el certificado no sean modificados y estén seguros|`sudo chmod 0600 /etc/ssl/certs/proftpd.crt`|
|*|`sudo useradd -m -s /bin/bash [nombre de usuario]`|para crear los usuarios|`sudo useradd -m -s /bin/bash [nombre de usuario]`|
|*|`sudo passwd [usuario]`|para asignamos contraseña|`sudo passwd [usuario]`|
|*|`sudo snap install nextcloud`|para instalar nextcloud|`sudo snap install nextcloud`|
|*|`snap changes nextcloud`|para hacer snapshots|`snap changes nextcloud`|
|*|`sudo nextcloud.manual-install user contraseña`|para crear usuario con sontraseña|`sudo nextcloud.manual-install user contraseña`|
|*|`sudo nextcloud.occ config:system:set trusted_domains 1 --value=nombre del dominio`|para ingresar el dominio y unirlos|`sudo nextcloud.occ config:system:set trusted_domains 1 --value=nombre del dominio`|
|*|`sudo ufw allow 80,443/tcp`|permitir la entrada de puertos|`sudo ufw allow 80,443/tcp`|
|*|`sudo nextcloud.enable-https lets-encrypt`|para iniciar la conexion con NextXloud|`sudo nextcloud.enable-https lets-encrypt`|
|*|`sudo cat /var/lib/docker/volumes/nextcloud_aio_mastercontainer/_data/data/configuration.json | grep password`|para poder saber la contraseña|`sudo cat /var/lib/docker/volumes/nextcloud_aio_mastercontainer/_data/data/configuration.json | grep password`|
|*|`sudo apt-get install samba`|para poder manejar los documentos tipo SMB|`sudo apt-get install samba`|
|*|`sudo systemctl stop nmbd.service`|parar los servicios .nmbd|`sudo systemctl stop nmbd.service`|
|*|`sudo systemctl disable nmbd.service`|para deshabilitar los servicios .nmbd|`sudo systemctl disable nmbd.service`|
|*|`ip link`|para descubrir el link de la ip|`ip link`|
|*|`sudo mv /etc/samba/smb.conf /etc/samba/smb.conf.orig`|para mover archivos|`sudo mv /etc/samba/smb.conf /etc/samba/smb.conf.orig`|
|*|`sudo nano /etc/samba/smb.conf`|para configurar algunos aspectos|`sudo nano /etc/samba/smb.conf`|
|*|`sudo mkdir /samba/  && sudo chown :sambashare /samba/`|para crear usuarios|`sudo mkdir /samba/  && sudo chown :sambashare /samba/`|
|*|`sudo adduser --home /samba/usuario --no-create-home --shell /usr/sbin/nologin --ingroup sambashare usuario`|mas usuarios|`sudo adduser --home /samba/usuario --no-create-home --shell /usr/sbin/nologin --ingroup sambashare usuario`|
|*|`sudo chown usuario:sambashare /samba/usuario/  &&  “sudo chmod 2770 /samba/usuario/`|para dar acceso a los usuarios|`sudo chown usuario:sambashare /samba/usuario/  &&  “sudo chmod 2770 /samba/usuario/`|
|*|`sudo smbpasswd -a usuario”  &&  “sudo smbpasswd -e usuario`|para meter usuarios al servidor|`sudo smbpasswd -a usuario”  &&  “sudo smbpasswd -e usuario`|
|*|`sudo mkdir /samba/everyone`|para crear admin|`sudo mkdir /samba/everyone`|
|*|`sudo adduser --home /samba/everyone --no-create-home --shell /usr/sbin/nologin --ingroup sambashare admin`|para crear admin|`sudo adduser --home /samba/everyone --no-create-home --shell /usr/sbin/nologin --ingroup sambashare admin`|
|*|`sudo chown admin:sambashare /samba/everyone/`|para crear admin|`sudo chown admin:sambashare /samba/everyone/`|
|*|`sudo chmod 2770 /samba/everyone/`|para crear admin|`sudo chmod 2770 /samba/everyone/`|
|*|`sudo smbpasswd -a admin`|para crear admin|`sudo smbpasswd -a admin`|
|*|`sudo usermod -G admins usuario`|para crear admin|`sudo usermod -G admins usuario`|
|*|`sudo nano /etc/samba/smb.conf`|para ingresar los usuarios|`sudo nano /etc/samba/smb.conf`|
|*|`sudo apt-get install smbclient`|para instalar el server|`sudo apt-get install smbclient`|
|*|`bash openvpn-install.sh`|para poder usar el root|`bash openvpn-install.sh`|
|*|`cd /etc/openvpn/`|para poder ir a esa dirección|`cd /etc/openvpn/`|
|*|`nano /usr/share/doc/openvpn/examples/sample-config-files/client.conf`|va a aparecer una pantalla, se debe de reemplazar por el Public IP|`nano /usr/share/doc/openvpn/examples/sample-config-files/client.conf`|
|*|`cd ~/ `|para verificar los clientes creados|`cd ~/ `|
|*|`sudo systemctl restart openvpn-server@server.service`|para reiniciar el OpenVPN|`sudo systemctl restart openvpn-server@server.service`|
|*|`sudo systemctl status openvpn-server@server.service`|para revisar que esté corriendo|`sudo systemctl status openvpn-server@server.service`|
|*|`scp nombremaquina@publicIP:/home/nombrecliente.ovpn`|para revisar que el cliente haya sido creado en los documentos|`scp nombremaquina@publicIP:/home/nombrecliente.ovpn`|
|*|`cp nombre documento /dondeVa/`|para mover los clientes que no esten en el lugar adecuado|`cp nombre documento /dondeVa/`|
|*|`sudo apt update && sudo apt upgrade -y`|para actualizar el sistema e instalar los últimos paquetes|`sudo apt update && sudo apt upgrade -y`|
|*|`sudo apt install kde-plasma-desktop`|es el que va a instalar Plasma en nuestra máquina virtual|`sudo apt install kde-plasma-desktop`|
|*|`sudo apt install latte-dock`|para la descarga de latte|`sudo apt install latte-dock`|
|*|`flatpak install https://flathub.org/repo/appstream/org.gimp.GIMP.flatpakref`|para instalar flatpak desde la terminal|`flatpak install https://flathub.org/repo/appstream/org.gimp.GIMP.flatpakref`|
