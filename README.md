# 🧠 UNet Polyp Segmentation SaaS  
## Plataforma Web de Inteligencia Artificial para Segmentación Automática de Pólipos

🔗 **Repositorio GitHub:** https://github.com/TU_USUARIO/unet-polyp-segmentation-saas  
🌐 **Aplicación Web (local):** http://127.0.0.1:8000  
📄 **Documentación API (Swagger):** http://127.0.0.1:8000/docs  
📘 **Documentación API (ReDoc):** http://127.0.0.1:8000/redoc  

---

## 1. Introducción

La detección temprana de pólipos colorrectales es un factor clave en la prevención del cáncer colorrectal, una de las principales causas de mortalidad a nivel mundial. En los procedimientos endoscópicos tradicionales, la identificación de pólipos depende en gran medida de la experiencia del especialista, lo que introduce variabilidad humana y posibles errores de omisión.

En este contexto, la **Inteligencia Artificial**, y en particular los modelos de **Deep Learning**, han demostrado un alto potencial para asistir al personal médico mediante herramientas de apoyo al diagnóstico. Entre estas técnicas, la **segmentación semántica de imágenes** permite identificar de forma precisa regiones de interés dentro de imágenes médicas, facilitando la visualización y el análisis clínico.

El presente proyecto propone el desarrollo de una **aplicación web tipo SaaS (Software as a Service)** que integra un modelo de **segmentación UNet** entrenado para identificar pólipos en imágenes endoscópicas, permitiendo su uso a través de una interfaz web accesible, segura y escalable.

---

## 2. Justificación del Proyecto

Este proyecto surge de la necesidad de:
- Integrar modelos de Inteligencia Artificial en soluciones web reales
- Demostrar la viabilidad técnica y económica de un producto basado en IA
- Aplicar conocimientos de Ingeniería Biomédica, Deep Learning y desarrollo de software
- Simular un producto comercializable en el sector salud

La implementación de una solución SaaS permite:
- Centralizar el modelo de IA
- Facilitar su uso sin necesidad de instalación local por parte del usuario final
- Escalar el servicio a múltiples usuarios o instituciones médicas
- Integrar mecanismos de autenticación y control de acceso

---

## 3. Objetivos

### 3.1 Objetivo General
Desarrollar una aplicación web funcional que consuma un servicio de Inteligencia Artificial para la segmentación automática de pólipos en imágenes endoscópicas, siguiendo una arquitectura SaaS.

### 3.2 Objetivos Específicos
- Entrenar e integrar un modelo UNet para segmentación de imágenes médicas
- Implementar un backend robusto utilizando FastAPI
- Diseñar una interfaz web para la carga de imágenes y visualización de resultados
- Implementar autenticación de usuarios con tokens JWT
- Evaluar la viabilidad financiera del proyecto mediante métricas VAN, TIR y Payback
- Documentar el sistema de forma profesional

---

## 4. Modelo de Inteligencia Artificial

### 4.1 Arquitectura UNet
El modelo utilizado se basa en la arquitectura **UNet**, ampliamente empleada en segmentación biomédica debido a su capacidad para capturar contexto global y detalles locales.

Características principales:
- Arquitectura encoder-decoder
- Conexiones tipo skip-connection
- Optimizada para segmentación semántica
- Alta precisión en imágenes médicas

### 4.2 Proceso de Entrenamiento
El modelo fue entrenado previamente en un entorno de Google Colab utilizando:
- TensorFlow y Keras
- Dataset de imágenes endoscópicas con máscaras
- Normalización de imágenes
- Función de pérdida adecuada para segmentación binaria

El resultado del entrenamiento fue almacenado en un archivo `.h5`, el cual es cargado directamente por el backend para realizar inferencia.

---

## 5. Arquitectura del Sistema

La arquitectura del sistema sigue un enfoque modular:

### 5.1 Backend
- **Lenguaje:** Python
- **Framework:** FastAPI
- **Servidor ASGI:** Uvicorn
- **ORM:** SQLAlchemy
- **Base de Datos:** SQLite
- **Autenticación:** JWT
- **Carga del modelo:** TensorFlow / Keras

El backend expone una API REST que permite:
- Registro y autenticación de usuarios
- Gestión de sesiones
- Procesamiento de imágenes
- Inferencia del modelo de IA

### 5.2 Frontend
- HTML5
- TailwindCSS
- Formularios web
- Interfaz clara e intuitiva
- Visualización directa de resultados de segmentación

El frontend se comunica con el backend mediante solicitudes HTTP, simulando el comportamiento real de un producto SaaS.

---

## 6. Funcionalidades del Sistema

La plataforma implementa las siguientes funcionalidades:

### 6.1 Gestión de Usuarios
- Registro de usuario
- Inicio de sesión
- Cierre de sesión
- Almacenamiento seguro de contraseñas

### 6.2 Servicio de Predicción
- Subida de imágenes endoscópicas
- Preprocesamiento automático
- Ejecución del modelo UNet
- Generación de máscara binaria
- Descarga o visualización del resultado

### 6.3 Documentación Automática
- Swagger UI
- ReDoc
- Especificación OpenAPI

---

## 7. Seguridad

El sistema implementa medidas básicas de seguridad:
- Hashing de contraseñas
- Autenticación basada en tokens
- Separación de rutas públicas y privadas
- Control de acceso a servicios de predicción

Esto simula un entorno profesional de producción.

---

## 8. Análisis Financiero

El proyecto fue evaluado como una solución rentable mediante:
- **VAN (Valor Actual Neto):** Evaluación del valor presente del proyecto
- **TIR (Tasa Interna de Retorno):** Medición de rentabilidad
- **Payback:** Tiempo de recuperación de la inversión

Los resultados indican que una plataforma SaaS de este tipo podría ser económicamente viable al ofrecer servicios de apoyo diagnóstico a clínicas y hospitales.

---

## 9. Despliegue

- **Tipo:** Local
- **Entorno:** Anaconda
- **Ejecución del servidor:**
  ```bash
  uvicorn app.main:app --reload

## 10. Resultados Obtenidos

- **Aplicación web funcional

- **Integración exitosa del modelo UNet

- **Segmentación automática correcta

- **Interfaz amigable

- **Cumplimiento de requisitos académicos y técnicos

## 11. Limitaciones y Trabajo Futuro

- **Integración con bases de datos médicas reales

- **Despliegue en la nube

- **Mejora del modelo con datasets más amplios

- **Inclusión de métricas clínicas

- **Cumplimiento de normativas médicas

## 12. Conclusiones

Este proyecto demuestra que es posible integrar de manera efectiva modelos de Inteligencia Artificial en aplicaciones web reales, creando soluciones escalables, seguras y con potencial comercial. La combinación de Deep Learning, desarrollo web y análisis financiero permite evaluar no solo la viabilidad técnica, sino también el impacto práctico del sistema.

## 13. Autora

Amber Grijalba
Ingeniería Biomédica
Inteligencia Artificial
Universidad Latina de Panamá

## 14. Licencia

Proyecto académico con fines educativos.



