# OPEMIP - Automatización de Reportes con IA

## Descripción del proyecto
Este proyecto piloto tiene como objetivo modernizar y automatizar la gestión de reportes diarios de maquinaria y personal, eliminando la necesidad de entrada de datos manual. Utiliza tecnologías de **Inteligencia Artificial (IA)** para un sistema de **Reconocimiento Óptico de Caracteres (OCR)** que extrae datos directamente de formularios en imágenes.

### Objetivos Clave
- **Digitalización de la Comunicación:** Transformar la gestión de reportes de formatos tradicionales (papel, mensajería) a una plataforma centralizada y automatizada.
- **Eficiencia Operativa:** Reducir errores y el tiempo dedicado a la consolidación manual de datos.
- **Análisis de Datos Mejorado:** Centralizar la información en Google Sheets para facilitar el análisis y la generación de reportes automáticos, lo que permite una toma de decisiones más rápida y precisa.

### Metodología
El sistema está diseñado para:
1. **Capturar imágenes** de los reportes diarios enviados por WhatsApp.
2. **Procesar las imágenes** utilizando un modelo de IA para extraer información clave.
3. **Escribir automáticamente los datos** en hojas de cálculo de Google Sheets.
4. **Ejecutar macros** para aplicar el formato, las reglas de negocio y las validaciones de manera automática.

### Estado Actual
Actualmente, el proyecto se encuentra en su fase piloto para demostrar la viabilidad y los beneficios de la automatización, con miras a una posterior implementación a gran escala.

---

## Tecnologías Utilizadas
- **Coolify:** Plataforma de despliegue y alojamiento.
- **n8n:** Herramienta de código abierto para la creación de flujos de trabajo de automatización.
- **OpenAI:** Proveedor del modelo de IA para el servicio de OCR.
- **Google Sheets:** Plataforma para la gestión y visualización de los datos extraídos.
- **GitHub:** Repositorio para la gestión y el control de versiones de los flujos de trabajo.

---

## Flujos de Trabajo (Workflows)
Los flujos de trabajo de n8n están organizados en archivos JSON dentro de este repositorio. Cada archivo representa una automatización específica:

- **`FORM PERSONAL NUEVO.json`**: Flujo para el registro de nuevos empleados.
- **`OPERADORES OPEMIP.json`**: Automatización para el procesamiento de reportes de operadores.
- **`CONDUCTORES OPEMIP.json`**: Automatización para el procesamiento de reportes de conductores.
- **`REPORTE 10AM.json`**: Flujo de trabajo programado para generar reportes a las 10:00 AM.
