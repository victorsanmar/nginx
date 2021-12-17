# Instalación Nginx

Para instalar **Nginx en Debian 10 Buster** usaremos el repositorio de la propia distribución. Por tanto, uno de los primeros pasos será actualizar la información de los paquetes disponibles en el repositorio:

``` ruby 
sudo apt update
```

Ya tenemos actualizada la información de los repositorios de Debian 10, así que es el momento de instalar el paquete nginx con apt:

``` ruby 
sudo apt -y install nginx
```

Tras la instalación del paquete y sus dependencias se crea un nuevo servicio llamado nginx.service o nginx en su versión corta. Este servicio queda activado para arrancar automáticamente con el sistema y también se ha iniciado al finalizar la instalación, como puedes comprobar con el comando **systemctl status nginx**:

![nginx](https://github.com/victorsanmar/nginx/blob/main/imagenes/status.PNG)

En el caso de tener activado el firewall UFW en Debian 10, si quieres acceder al servicio web desde red será necesario añadir algunas reglas.

Para el servicio estándar HTTP (puerto 80/TCP):

``` ruby 
sudo ufw allow http
```

Y si vas a servir contenido seguro, mediante HTTPS (puerto 443/TCP):

``` ruby 
sudo ufw allow https
```
