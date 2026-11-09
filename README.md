# AI-Powered-Workflow-Automation
AI-powered customer request automation using n8n, OpenAI, Gmail and Google Sheets
# Automatización de solicitudes de clientes con IA y n8n

## Descripción del proyecto

Proyecto de automatización de procesos empresariales mediante n8n e inteligencia artificial.

El sistema recibe solicitudes de clientes, utiliza un agente de IA basado en OpenAI para generar respuestas personalizadas por correo electrónico, automatiza su envío mediante Gmail y registra los datos de los contactos en Google Sheets.

## Objetivos

- Automatizar la atención inicial de solicitudes comerciales.
- Generar respuestas personalizadas mediante inteligencia artificial.
- Reducir tareas manuales y tiempos de gestión.
- Registrar y organizar nuevos contactos comerciales.
- Diseñar un flujo de trabajo modular y ampliable.

## Tecnologías utilizadas

- **n8n:** diseño y orquestación de workflows.
- **OpenAI (GPT-4.1-mini):** generación de respuestas mediante IA.
- **Gmail:** envío automatizado de correos electrónicos.
- **Google Sheets:** almacenamiento y registro de nuevos leads.
- **Docker:** ejecución local de n8n.
- **JSON y expresiones de n8n:** tratamiento, estructuración y extracción de datos.

## Arquitectura del workflow

El proceso está compuesto por los siguientes nodos:

1. **Formulario:** entrada de datos de las solicitudes de clientes.
2. **Wait:** gestión de la espera dentro del flujo.
3. **Agente de IA:** interpretación de la solicitud y generación de un correo personalizado.
4. **Gmail:** envío automático del correo, separando el asunto y el cuerpo del mensaje.
5. **Google Sheets:** registro de los nuevos contactos comerciales.

## Funcionalidades implementadas

- Generación dinámica de asuntos y cuerpos de correo.
- Respuestas personalizadas mediante inteligencia artificial.
- Generación de respuestas con estructura JSON.
- Extracción de datos mediante expresiones de n8n.
- Integración y envío automatizado mediante Gmail.
- Registro de leads en una hoja de cálculo.

## Instalación y ejecución

El proyecto se ha desarrollado con n8n Self-hosted mediante Docker.

Para iniciar el contenedor de n8n:

```bash
docker start n8n
```

Acceder desde el navegador:

```text
http://localhost:5678
```

Es necesario configurar las credenciales propias de OpenAI, Gmail y Google Sheets.

## Seguridad

Las credenciales y claves API se gestionan mediante el sistema de credenciales de n8n.

No se deben incluir claves API, tokens, contraseñas ni datos personales en los archivos públicos del repositorio.

## Posibles mejoras futuras

- Integración con plataformas de reservas como Cal.com.
- Incorporación de nuevos canales de entrada.
- Seguimiento automatizado de solicitudes.
- Clasificación y priorización de leads.
- Incorporación de métricas y seguimiento de resultados.

## Competencias demostradas

- Diseño y desarrollo de workflows.
- Automatización de procesos empresariales.
- Integración de APIs y servicios externos.
- Aplicación de inteligencia artificial generativa.
- Tratamiento de datos estructurados mediante JSON.
- Integración de herramientas digitales.
- Despliegue local de aplicaciones mediante Docker.

## Estado del proyecto

Proyecto funcional desarrollado como parte de mi portfolio práctico de inteligencia artificial aplicada y automatización de procesos.

## Autora

Proyecto personal desarrollado como parte de mi formación en inteligencia artificial aplicada y automatización de procesos.
