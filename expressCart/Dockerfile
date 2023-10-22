# Usa la imagen base de Node.js 14
FROM node:14

# Establece el directorio de trabajo en /var/expressCart
WORKDIR /var/expressCart

# Copia tus archivos de la aplicación
COPY lib/ /var/expressCart/lib/
COPY bin/ /var/expressCart/bin/
COPY config/ /var/expressCart/config/
COPY public/ /var/expressCart/public/
COPY routes/ /var/expressCart/routes/
COPY views/ /var/expressCart/views/
COPY app.js /var/expressCart/
COPY package.json /var/expressCart/
COPY deploy.js /var/expressCart/

# Instala las dependencias de la aplicación
RUN npm install

# Expone el puerto 1111
EXPOSE 1111

# Establece el comando de inicio de la aplicación
CMD ["npm", "start"]
