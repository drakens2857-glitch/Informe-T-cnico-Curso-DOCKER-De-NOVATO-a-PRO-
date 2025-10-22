# Informe-T-cnico-Curso-DOCKER-De-NOVATO-a-PRO-

##  Objetivo del informe
Este informe documenta los conceptos clave aprendidos en el curso “Docker de Novato a Pro”, reflexiona sobre su aplicabilidad en entornos backend modernos, y presenta un ejemplo práctico con FastAPI y Docker Compose. El propósito es consolidar conocimientos sobre contenedores, imágenes, redes y orquestación de servicios.

---

##  Resumen de conceptos por sección del curso

### 1. ¿Qué es Docker?
- Docker es una plataforma para empaquetar aplicaciones en contenedores ligeros, portables y aislados.
- Diferencias clave entre contenedores y máquinas virtuales: menor consumo de recursos, arranque más rápido, y mayor portabilidad.

### 2. Instalación y primeros comandos
- Instalación en Windows, macOS y Linux.
- Comandos básicos: `docker run`, `docker ps`, `docker stop`, `docker rm`, `docker images`, `docker build`.

### 3. Imágenes y contenedores
- Las imágenes son plantillas inmutables para crear contenedores.
- Se pueden obtener desde Docker Hub o construir con `Dockerfile`.

### 4. Dockerfile
- Script que define cómo construir una imagen personalizada.
- Instrucciones clave: `FROM`, `WORKDIR`, `COPY`, `RUN`, `CMD`.

### 5. Volúmenes
- Permiten persistir datos fuera del contenedor.
- Uso de `docker volume create`, `-v` y montaje de carpetas locales.

### 6. Redes Docker
- Comunicación entre contenedores mediante redes bridge, host y overlay.
- Comando: `docker network create`.

### 7. Docker Compose
- Herramienta para definir múltiples servicios en un solo archivo `docker-compose.yml`.
- Comandos: `docker-compose up`, `down`, `build`, `logs`.

---

##  Reflexiones personales

###  Ventajas
- **Portabilidad total**: los contenedores funcionan igual en cualquier entorno.
- **Aislamiento de servicios**: ideal para microservicios y pruebas independientes.
- **Despliegue rápido**: facilita la automatización y CI/CD.
- **Reproducibilidad**: el entorno se define por código, lo que evita el clásico “en mi máquina sí funciona”.

###  Desafíos
- **Curva de aprendizaje**: requiere entender bien conceptos como imágenes, volúmenes y redes.
- **Gestión avanzada**: orquestar múltiples servicios puede volverse complejo sin herramientas como Docker Compose o Kubernetes.

###  Aplicación práctica
Docker es especialmente útil en proyectos backend con múltiples servicios (API, base de datos, frontend). Planeo usarlo para encapsular APIs con FastAPI, bases de datos PostgreSQL, y dashboards con Streamlit.

---

##  Ejemplo práctico: API con FastAPI + Docker

### Estructura del proyecto
