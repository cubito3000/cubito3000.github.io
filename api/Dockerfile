# Usar una imagen oficial de Python ligera
FROM python:3.11-slim

# Crear una carpeta de trabajo dentro del contenedor
WORKDIR /app

# Copiar el archivo de dependencias primero
COPY requirements.txt .

# Instalar las dependencias
RUN pip install --no-cache-dir -r requirements.txt

# Copiar el resto del código de la API
COPY . .

# Indicar que la API escucha en el puerto 3000
EXPOSE 3000

# Comando de arranque especificado en la guía
CMD ["gunicorn", "-b", "0.0.0.0:3000", "app:app"]