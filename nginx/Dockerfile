#Usare una imagen Docker existente como base
FROM nginx

#Asignar Directorio de Trabajo
WORKDIR '/app'

#Descargar dependencia
COPY ./default.conf /etc/nginx/conf.d/default.conf
COPY ./htpasswd /etc/nginx/.htpasswd
# COPY ./ssl/ /etc/nginx/ssl/
COPY ./ssl /etc/nginx/
EXPOSE 443