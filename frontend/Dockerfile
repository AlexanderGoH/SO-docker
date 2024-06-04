# Usar una imagen base de Node.js para construir la app Angular
FROM node:18.20-alpine as build-step

# Crear dirección de trabajo
RUN mkdir -p /app

# Asignar directorio de trabajo
WORKDIR /app

# Copiar package.json y package-lock.json
COPY package.json /app

# Instalar dependencias
RUN npm install

# Copiar el resto del código
COPY . .

# Construir la app Angular
RUN npm run build --prod

# Usar una imagen base de Nginx para servir la app
FROM nginx:latest

# Copiar los archivos construidos desde el primer contenedor
COPY --from=build-step /app/dist/prograweb/browser /usr/share/nginx/html

# Exponer el puerto en el que Nginx servirá la app
EXPOSE 80