# Imagen base de Ubuntu
FROM ubuntu:20.04

# Instala netcat
RUN apt-get update && apt-get install -y netcat && rm -rf /var/lib/apt/lists/*

# Comando para conectarse al servidor y enviar un mensaje
CMD ["sh", "-c", "echo 'Hola desde el cliente!' | nc 192.168.67.10 2025"]

