FROM nginx:alpine

# Copiar la configuración del servidor
COPY web/nginx.conf /etc/nginx/conf.d/default.conf

# Copiar tu página y el script
COPY index.html /usr/share/nginx/html/
COPY libro-de-visitas.js /usr/share/nginx/html/