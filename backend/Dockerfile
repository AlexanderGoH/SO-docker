# Usar imagen base de Node.js
FROM node:20.14.0

# Crear dirección de trabajo
RUN mkdir -p /app

# Crear directorio de trabajo
WORKDIR /app

#Copiar package.json y package.lock.json
COPY package*.json ./

# Instalar dependencias
RUN npm install

# Instalar nodemon globalmente
RUN npm install -g nodemon

# Copiar el resto del código
COPY . .

# Exponer el puerto en el que la app esuchará
EXPOSE 3000

#Comando para correr la app
CMD ["npm", "run", "start:dev"]