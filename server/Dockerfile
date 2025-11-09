# Usa una imagen base de Ubuntu
FROM ubuntu:20.04

# Instala netcat para pruebas TCP
RUN apt-get update && apt-get install -y netcat && rm -rf /var/lib/apt/lists/*

# Expone el puerto 2025
EXPOSE 2025

# Comando para mantener un servidor TCP escuchando
CMD ["sh", "-c", "while true; do nc -l -p 2025 -k -v; done"]
