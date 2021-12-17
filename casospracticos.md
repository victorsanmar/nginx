# Casos prácticos

## Versión de Nginx instalado.
 
``` ruby 
apt policy nginx
```

![casos](https://github.com/victorsanmar/nginx/blob/main/imagenes/version.PNG)

## Ficheros de configuración.

Fichero de configuración para balancear

[load-balancing](https://github.com/victorsanmar/nginx/blob/main/load-balancing.conf)

Fichero de configuración del servidor

[default](https://github.com/victorsanmar/nginx/blob/main/default)

## Página web por defecto:

Para cambiar el contenido de nuestra página haremos lo siguiente:

``` ruby 
echo "EJEMPLO DE NGINX PARA GITHUB" >>/var/www/nginx/index.html
```

Comprobamos nuestra pagina poniendo localhost en el navegador por el puerto configurado para entrar

![localhost](https://github.com/victorsanmar/nginx/blob/main/imagenes/localhost.PNG)

## Aqui te dejo una pequeña guia sobre nginx y SSL

[Nginx y SSL](https://github.com/victorsanmar/script-lamp/blob/main/NGINX%20ssl%20y%20balanceo.pdf)
