# Imagen base de Ubuntu
FROM ubuntu:20.04

# Instala netcat
RUN apt-get update && apt-get install -y netcat && rm -rf /var/lib/apt/lists/*

# Expone el puerto TCP
EXPOSE 2025

# Comando para escuchar conexiones en el puerto 2025
CMD ["sh", "-c", "echo 'Servidor TCP iniciado...' && nc -lk -p 2025"]

