FROM debian:bullseye

# Instala Python e pip
RUN apt-get update && apt-get install -y python3 python3-pip && apt-get clean

# Directorio de traballo
WORKDIR /app

# Copiar requirements para instalar dependencias
COPY requirements.txt .

# Instalar dependencias
RUN pip3 install -r requirements.txt

# O código se cargará con bind mount, non fai falta copiar aquí o app.py

# Comando por defecto para executar a app
CMD ["python3", "app.py"]
