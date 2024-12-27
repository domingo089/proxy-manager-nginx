# proxy-manager
Proxi-Manager - Docker-compose

Ver en "Localhost:81"

Usuario:    admin@example.com

Password: changeme

Cómo instalar NGINX Proxy Manager usando docker-compose
 

¿Qué es NGINX Proxy Manager?
 

Es un Hosts proxy para exponer los servicios web en tu red · SSL gratuito con Let's Encrypt · Diseñado pensando en la seguridad · Perfecto para redes domésticas y conectarte desde cualquier lugar de forma segura.

El administrador de proxy NGINX es un sistema de administración de proxy inverso, que se basa en NGINX con una interfaz de usuario web agradable y limpia.

SSL gratis - El soporte integrado de Let's Encrypt te permite proteger tus servicios web sin costo alguno para tí.

Los certificados incluso se renuevan solos.

Sitio web de NGINX Proxy Manager.

 

Instalación de NGINX Proxy Manager:
 

Puedes descargar el archivo de github.

Si lo prefieres puedes hacer la instalación ejecutando este comando dentro de tu carpeta "docker"

1
git clone https://github.com/jmlcas/proxy-manager
 y luego como siempre 

1
docker-compose up -d
Ahora ya puedes abrir en el navegador "localhost:81"

Y te pedirá estos datos:

Email: admin@example.com
Password: changeme

login-pm

 

NGINX Proxy Manager  se puede instalar perfectamente en una Raspberry Pi 4.

 

Antes de utilizar esta aplicación deberás seguir todas estas instrucciones:

Esto es una muestra de lo realizado en el vídeo ( te aconsejo lo veas entero para entender mejor este artículo).

 

puertos-1

 

Agregar puertos al Firewall del VPS
puertos-clouding
VPS utilizado: clouding

 

Crear sub-dominios en el Hosting
subdominios-hostinger

CPanel utilizado: Hostinger

 

Apuntar los sub-dominios al registro DNS correcto
dns-hostinger

 

En el vídeo no aparece, pero acuérdate, debes crear también el subdominio "proxy" para "proxy-manager", abrir los puertos 80,81 y 443 y apuntar el subdominio a la IP correspondiente.  

 

Configurar Nginx Proxy-Manager
config-proxy

 

Configurar https(SSL) en WordPress
ssl-wp

 

Configurar Heimdall
config-heim

 

En este artículo he agregado 5 aplicaciones web, pero puedes agregar cuantas quieras. Por ejemplo en esta imagen están las que yo tengo instaladas en un servidor.

heimdall-lab

 

Enlaces de descarga de las app utilizadas en el vídeo:

Web WordPress

Glances

Heimdall

Portainer

Nextcloud

 

Y listo, ya tienes tus app instaladas en un solo VPS con SSL, basándote en un solo dominio y varios subdominios.
