# Laboratorio: Práctica de Serverless con OpenFaaS

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![OpenFaaS](https://img.shields.io/badge/OpenFaaS-00B5AD?style=for-the-badge&logo=openfaas&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

---

## Descripción del Proyecto

Este proyecto corresponde al **Laboratorio: Práctica de Serverless**, desarrollado como parte de las actividades prácticas de la asignatura de **Introducción al Cómputo en la Nube**.

La aplicación implementa un entorno Serverless local mediante **OpenFaaS**, utilizando **Docker Desktop** y **Kubernetes** para desarrollar, desplegar y ejecutar una función en **Python** (`python3-http`) capaz de procesar solicitudes HTTP mediante un formulario web.

Durante la práctica se genera un archivo JSON descargable que contiene los datos registrados, un identificador único (UUID), información del entorno de ejecución y una firma criptográfica SHA-256.

---

## Información del Estudiante

| Campo | Información |
|---|---|
| Nombre(s) | Roberto Ernesto |
| Apellido(s) | Ramos Martinez |
| Correo Electrónico | reramoz@gmail.com |
| Asignatura | Introducción al Cómputo en la Nube |
| Tutor | Vladimir Mate |
| Fecha de Entrega | 06/11/2026 |

---

## Objetivo del Laboratorio

Implementar un entorno Serverless local mediante OpenFaaS para desarrollar, desplegar y ejecutar una función Python que permita registrar información mediante un formulario web, generar identificadores únicos y producir un archivo JSON descargable como resultado de la ejecución del servicio.

---

## Competencia

Implementa servicios Serverless en entornos cloud simulados mediante OpenFaaS, Docker y Kubernetes, desarrollando funciones en Python capaces de procesar solicitudes HTTP, gestionar información estructurada y generar archivos de salida, aplicando los fundamentos del modelo Functions as a Service (FaaS).

---

## Tecnologías y Herramientas Utilizadas

- **Docker Desktop**: Infraestructura de contenedores y motor de ejecución.
- **Kubernetes (Kubeadm)**: Orquestador local de contenedores.
- **OpenFaaS / OpenFaaS CLI**: Plataforma de Functions as a Service (FaaS) y herramienta de administración de funciones.
- **Helm**: Gestor de paquetes para la instalación de OpenFaaS en Kubernetes.
- **Python (Template `python3-http`)**: Lenguaje de programación para la función Serverless.
- **Visual Studio Code**: Entorno de desarrollo integrado.
- **PowerShell**: Terminal de comandos en Windows.

---

## Estructura del Proyecto

```text
laboratorio-serverless/
│
├── build/
│   └── registro-serverless/
│       ├── function/
│       ├── Dockerfile
│       ├── index.py
│       └── requirements.txt
│
├── registro-serverless/
│   ├── handler.py
│   ├── handler_test.py
│   ├── requirements.txt
│   └── tox.ini
│
├── template/
│   └── python3-http/
│
├── .gitignore
├── README.md
├── stack.yaml
└── registro_*.json
