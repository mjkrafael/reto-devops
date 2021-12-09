#Usare una imagen Docker existente como base
FROM node:alpine

#Asignar Directorio de Trabajo
WORKDIR '/app'

#Descargar e instalar dependencia
COPY package.json .

RUN npm install

COPY . .

RUN npm run test

#Tareas del docker al iniciar
CMD ["node", "index.js"]


# #Usare una imagen Docker existente como base
# FROM node:alpine

# # Instalat Git - clonar repositorio
# RUN apk add git \
#     && git clone https://gitlab.com/clm-public/reto-devops.git

# #Asignar Directorio de Trabajo
# WORKDIR '/reto-devops'

# #Instalar / Testear dependencia
#  RUN npm install \
#     && npm run test

# #Tareas del docker al iniciar
# CMD ["node", "index.js"]


