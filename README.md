# Cloud Resume Challenge

Este proyecto implementa una solución completa para el **Cloud Resume Challenge** utilizando los servicios de AWS. Incluye un sitio web estático alojado en S3, un backend sin servidor con AWS Lambda y API Gateway, una base de datos DynamoDB para el contador de visitantes y una infraestructura gestionada con AWS CloudFormation.

---

## 🏗️ Arquitectura

![Arquitectura del Proyecto](https://mi-url-de-imagen.com/diagrama.png) <!-- Agrega una URL si tienes un diagrama arquitectónico -->

1. **Frontend**:
   - Sitio web estático (HTML/CSS/JavaScript) alojado en Amazon S3.
   - Distribuido globalmente a través de Amazon CloudFront con HTTPS habilitado.
2. **Backend**:
   - API REST gestionada con Amazon API Gateway.
   - Función Lambda en Python para manejar el contador de visitantes.
3. **Base de Datos**:
   - Amazon DynamoDB para almacenar el contador de visitantes.
4. **Infraestructura**:
   - Gestionada como código (IaC) usando AWS CloudFormation.
5. **CI/CD**:
   - Pipelines de AWS CodePipeline para automatizar el despliegue.

---

## 🚀 Funcionalidades

- **Contador de Visitantes**: Incrementa cada vez que alguien accede al sitio web.
- **Hosting Seguro**: Todo el contenido estático está disponible a través de HTTPS.
- **Escalabilidad Automática**: Backend sin servidor que escala automáticamente para manejar picos de tráfico.
- **Integración Continua**: Despliegue automático del frontend y backend mediante CodePipeline.

---

## 📋 Requisitos

Antes de comenzar, asegúrate de tener lo siguiente:
- **Cuenta de AWS** configurada.
- **CLI de AWS** instalada y configurada.
- **Python 3.9+** instalado en tu máquina local.
- **Bucket S3** creado para almacenar artefactos (puede configurarse durante el despliegue).

---

## 🛠️ Implementación

### **1. Desplegar Infraestructura**
1. Clona este repositorio:
   ```bash
   git clone https://github.com/JonaPD/cloud-resume-challenge.git
   cd cloud-resume-challenge
