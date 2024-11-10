# **PYTHON HOLA MUNDO**

Este repositorio contiene un programa básico "Hola Mundo" escrito en Python, perfecto como introducción a la programación en Python.

## Descripción
El programa imprime el mensaje "Hola Mundo" en la consola, demostrando la sintaxis básica de Python y cómo ejecutar un script simple.

## Requisitos
- **Lenguaje**: Python 3.x
- **Requisitos adicionales**: Ninguno

## Cómo Clonar y Ejecutar
Para clonar este repositorio en tu máquina local, usa los siguientes comandos:
```bash
git clone https://github.com/<tu-usuario>/python-hola-mundo.git
cd python-hola-mundo
```

Para ejecutar el programa, simplemente usa:
```bash
python hello_world.py
```

## Estructura del Proyecto
```
python-hola-mundo/
│
├── hello_world.py     # Archivo principal del programa
└── README.md         # Este archivo
```

## Enlace de Docker Hub
**https://hub.docker.com/repository/docker/john2713/python-docker-hello-world/general**


## Dockerización
**Paso 1: Construir la Imagen Docker**
```bash
docker build -t python-hola-mundo .
```

**Paso 2: Etiquetar la Imagen**
```bash
docker tag python-hola-mundo <tu-usuario>/python-hola-mundo:latest
```

**Paso 3: Subir la Imagen a Docker Hub**
```bash
docker push <tu-usuario>/python-hola-mundo:latest
```

## Contenido del Dockerfile
```dockerfile
FROM python:3.8-slim
WORKDIR /app
COPY . .
CMD ["python", "hello_world.py"]
```

## Contribuir
Las contribuciones son bienvenidas. Por favor, siente libre de:
1. Hacer fork del proyecto
2. Crear una nueva rama (`git checkout -b feature/mejora`)
3. Hacer commit de tus cambios (`git commit -am 'Agrega nueva mejora'`)
4. Hacer push a la rama (`git push origin feature/mejora`)
5. Crear un Pull Request

## Licencia
Este proyecto está bajo la Licencia MIT.

---
*Recuerda reemplazar `<tu-usuario>` con tu nombre de usuario de GitHub o Docker Hub.*
