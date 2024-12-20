# Chatbot App con WebUI y Ollama (Usando Docker) 🤖🚀

Este proyecto implementa una aplicación de chatbot local utilizando WebUI y Ollama. La configuración se realiza completamente en contenedores Docker, lo que asegura un entorno limpio, reproducible y fácil de desplegar.

## 🌟 Características

•	🤖 Chatbot basado en LLMs: Interactúa con modelos avanzados de lenguaje.
•	💻 WebUI intuitiva: Interfaz gráfica para facilitar la interacción.
•	🔒 Despliegue local: Toda la aplicación se ejecuta en tu máquina, garantizando privacidad.
•	🐳 Aislamiento con Docker: Configuración y ejecución simplificada.

## 🛠️ Requisitos previos

1.	Docker instalado en tu máquina.
•	Descarga e instala Docker desde: https://www.docker.com/get-started
2.	Git para clonar el repositorio.
•	Instálalo desde: https://git-scm.com/

## 🚀 Instalación y configuración

1. Clona este repositorio:  
```plaintext
git clone https://github.com/tu-usuario/chatbot-docker-app.git
cd chatbot-docker-app
```

2.	Inicia los contenedores:
```plaintext
docker-compose up -d
```

3.	Accede a la aplicación:
•	Abre tu navegador y ve a: http://localhost:3000

4.	Para los contenedores:
```plaintext
docker-compose down
```

## 📂 Estructura del proyecto

```plaintext
chatbot-docker-app/
├── docker-compose.yml          # Configuración de múltiples servicios
├── backend/                    # Volumen con backend de WebUI
│   └── vector_db/              # DB de vectores y conversaciones
├── models/                     # Volumen con modelos de Ollama
│   ├── blobs/                  # Archivos estáticos de la WebUI
│   └── manifests/              # Servidor principal (Flask/FastAPI)
└── README.md                   # Este archivo
```
