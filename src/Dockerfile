# Usa una imagen base ligera
FROM node:20.9.0-alpine3.18

# Establece el directorio de trabajo
WORKDIR /app

# Copia únicamente los archivos necesarios para instalar dependencias
COPY package*.json ./

# Instala las dependencias en modo de producción para reducir el tamaño
RUN npm install --production

# Copia el resto del código fuente al contenedor
COPY . .

# Expone el puerto de la aplicación
EXPOSE 8080

# Define el comando de inicio
CMD ["node", "server.js"]
