# Así he creado mi propio servidor VPN para COMPARTIR NETFLIX, SPOTIFY y muchos más
## Script auto-install VPN Wireguard en Raspberry Pi

Guía de cómo instalar servidor VPN Wireguard en Raspberry Pi con un sencillo script. También haremos pruebas de conexión en Windows, Smart TV, Tablet y móvil.

![miniatura yt](https://github.com/JLalib/wireguard-install-sh/assets/57844755/7e96de92-fbe7-4ef4-8ab6-afd3334e255a)

Script auto-install VPN Wireguard

El script es válido para sistemas Linux, como Ubuntu, Debian, AlmaLinux, Rocky Linux, CentOS, Fedora, Raspbian OS, etc.

Este script le permitirá configurar su propio servidor VPN en no más de un minuto, incluso si no ha utilizado WireGuard antes. Ha sido diseñado para ser lo más discreto y universal posible.

Vídeo en YouTube de la configuración servidor VPN Wireguard.

⏭📼 Vídeo completo en Youtube https://bit.ly/3NKeL8K

Instalación

Descarga el script y ejecutalo como root.

wget https://git.io/wireguard -O wireguard-install.sh

En algunos casos, es necesario darle permisos de ejecución.

sudo chmod a+x wireguard-install.sh

Ahora, ejecuta el script.

sudo ./wireguard-install.sh

Durante la configuración, te preguntará varios ajustes de configuraciones.

![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/8df9d0a1-24db-496d-8a4e-8dbb8d738fd4)

Después escoge la interfaz donde se configurará la VPN, si tienes varias, normalmete es la de tu red local.

Indica tu IP pública o nombre dns. Te recomiendo tener un servicio como duckdns o no-ip. Posteriormente el puerto, que tendrás que abrir en tu router de Internet.

Escribe el nombre de tu "cliente".

Ahora los servidores DNS, puedes dejar los de tu red por defecto o bien seleccionar alguno de la lista.

Posteriormente, pasamos a crear los peers para nuestros usuarios. Este fichero de .config, es el que tenemos que copiar y enviar a los clientes que se conectarán a nuestra VPN desde sus dispositivos.
![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/4a26fd44-c095-49ab-9283-6810c2a912cd)

Aquí puedes escanear el QR desde la app Wireguard en Android o Iphone.

![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/c4f352cc-dc42-462c-9c4c-5024dbbf7822)

Usa este comando para copiar el fichero .conf en el directorio personal, actual u otro, para copiar a tu equipo windows, usa el programa WinSCP.

![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/be65e974-329b-4d8b-b327-4c9a10bf4e01)

Para crear más usuario con su fichero de configuración, es tan simple como volver a ejecutar el script.

![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/0d526e8f-13cf-495c-810e-c1f144f58d78)

![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/8cb72edf-bbf6-4e27-9f4e-58d1bd40b5c7)

Para visualizar el fichero .conf, puedes usar el comando cat
![image](https://github.com/JLalib/wireguard-install-sh/assets/57844755/f15c6f2e-a6d8-428f-b201-68ecb24d90a4)

Una vez que finalice, puede ejecutarlo nuevamente para agregar más usuarios, eliminar algunos de ellos o incluso desinstalar WireGuard por completo.

Para copiar el fichero a tu equipo Windows, puedes usar el programa WinSCP.

Enlaces de los instaladores

https://www.wireguard.com/install/

https://download.wireguard.com/windows-client/wireguard-installer.exe

https://itunes.apple.com/us/app/wireguard/id1451685025?ls=1&mt=12

https://play.google.com/store/apps/details?id=com.wireguard.android

https://itunes.apple.com/us/app/wireguard/id1441195209?ls=1&mt=8

Fuentes:

https://www.wireguard.com/

https://github.com/Nyr/wireguard-install

![wireguard](https://github.com/JLalib/wireguard-install-sh/assets/57844755/8720cc6b-fd3b-428c-a26f-0b3d3fd7ea2b)
