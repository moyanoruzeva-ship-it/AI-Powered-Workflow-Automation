# Automatización de solicitudes de clientes con IA y n8n

## Descripción del proyecto

Automatización de la gestión de solicitudes de clientes mediante n8n e inteligencia artificial.

El sistema recibe los datos de una solicitud, utiliza un agente de IA basado en OpenAI para generar una respuesta personalizada por correo electrónico, envía el mensaje automáticamente mediante Gmail e incluye un enlace de Cal.com para que el cliente pueda agendar una reunión. Además, registra los datos del contacto en Google Sheets.

## Objetivos

- Automatizar la atención inicial de solicitudes comerciales.
- Generar respuestas personalizadas mediante IA.
- Reducir tareas manuales y tiempos de gestión.
- Registrar y organizar nuevos contactos comerciales.
- Diseñar un flujo de trabajo modular y ampliable.

## Tecnologías utilizadas

- **n8n:** diseño y orquestación de workflows.
- **OpenAI (GPT-4.1-mini):** generación de respuestas mediante IA.
- **Gmail:** envío automatizado de correos electrónicos.
- **Cal.com:** enlace para facilitar la reserva de reuniones.
- **Google Sheets:** almacenamiento y registro de nuevos leads.
- **Docker:** ejecución local de n8n.
- **Expresiones y JSON:** tratamiento y estructuración de datos.

## Arquitectura del workflow

1. **Formulario:** entrada de datos de una solicitud de cliente.
2. **Wait:** gestión de la espera dentro del flujo.
3. **Agente de IA:** interpretación de la solicitud y generación de un correo personalizado.
4. **Gmail:** envío automático del correo, separando asunto y cuerpo del mensaje e incluyendo un enlace de Cal.com para agendar una reunión.
5. **Google Sheets:** registro de los nuevos contactos.

## Funcionalidades implementadas

- Generación dinámica de asuntos y cuerpos de correo.
- Respuestas personalizadas mediante inteligencia artificial.
- Salida estructurada en JSON.
- Extracción de datos mediante expresiones de n8n.
- Envío automatizado de emails.
- Inclusión de un enlace de Cal.com para facilitar la reserva de reuniones.
- Registro de leads en una hoja de cálculo.

## Instalación y ejecución

El proyecto se ha desarrollado con n8n Self-hosted mediante Docker.

Para ejecutar n8n localmente:

```bash
docker start n8n
```

Acceder desde el navegador:

```text
http://localhost:5678
```

Es necesario configurar las credenciales propias de OpenAI, Gmail y Google Sheets, así como adaptar los datos de entrada y el enlace de reservas.

## Seguridad

Las credenciales y claves API se gestionan mediante el sistema de credenciales de n8n.

No se deben incluir claves API, tokens, contraseñas ni datos personales en los archivos públicos del repositorio.

## Posibles mejoras futuras

- Integración con plataformas de reservas como Cal.com mediante un trigger independiente.
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

Proyecto funcional y desarrollado con fines de aprendizaje y portfolio profesional.

## Autora

Proyecto personal desarrollado como parte de mi formación en inteligencia artificial aplicada y automatización de procesos.
