# Práctica 2  
## Análisis de requerimientos y análisis de infraestructura

---

## 1. Integrantes del grupo
- Nombre completo - Carnet  
- Nombre completo - Carnet  
- Nombre completo - Carnet  
- Nombre completo - Carnet  
- Nombre completo - Carnet  

---

## 2. Introducción del caso

Una **empresa comercial pequeña**, con **20 empleados**, utiliza un sistema interno para:

- Almacenar documentos administrativos  
- Compartir archivos entre áreas  
- Registrar información básica de clientes  

Actualmente la empresa presenta los siguientes problemas:

- El sistema se vuelve lento cuando varios usuarios trabajan al mismo tiempo  
- Algunos documentos desaparecen o se sobrescriben  
- El sistema deja de funcionar de forma inesperada durante la jornada laboral  

La empresa:

- No cuenta con documentación técnica  
- No tiene personal especializado en TI  
- Describe los problemas únicamente desde su experiencia diaria  

---

## 3. Requerimientos seleccionados

### Requerimiento 1
**Descripción:**  
El sistema debe mantener tiempos de respuesta adecuados cuando los 20 usuarios trabajen simultáneamente.  

**Origen (necesidad):**  
Lentitud del sistema cuando varios usuarios acceden al mismo tiempo.

---

### Requerimiento 2
**Descripción:**  
El sistema debe garantizar la integridad y conservación de los documentos almacenados.  

**Origen (necesidad):**  
Desaparición y sobrescritura de documentos.

---

### Requerimiento 3
**Descripción:**  
El sistema debe asegurar disponibilidad continua durante la jornada laboral.  

**Origen (necesidad):**  
Interrupciones inesperadas del sistema.

---

## 4. Validación de requerimientos

### 4.1 Instrumento de recopilación utilizado

- **Tipo de instrumento:** Entrevista  
- **Justificación de la elección:**  
Se selecciona entrevista debido a que la empresa no posee conocimientos técnicos, por lo que permite profundizar y aclarar problemas expresados en lenguaje cotidiano.

---

### 4.2 Preguntas utilizadas

1. ¿En qué momentos del día el sistema presenta mayor lentitud?  
2. ¿Con qué frecuencia desaparecen o se sobrescriben documentos?  
3. ¿Qué áreas son las más afectadas por las fallas del sistema?  
4. ¿Cuánto tiempo permanece inactivo el sistema cuando falla?  
5. ¿Existe algún procedimiento actual para respaldar información?  

---

### 4.3 Resultado de la validación

| Requerimiento | ¿Es correcto? | ¿Es necesario? | ¿Es comprensible? | Observaciones |
|--------------|---------------|----------------|-------------------|---------------|
| Req. 1 | Sí | Sí | Sí | Impacta directamente la productividad. |
| Req. 2 | Sí | Sí | Sí | Afecta la seguridad de la información. |
| Req. 3 | Sí | Sí | Sí | Interrumpe las actividades comerciales. |

---

## 5. Priorización de requerimientos

### 5.1 Matriz de priorización

| Requerimiento | Impacto Operativo (Alto/Medio/Bajo) | Criticidad Técnica (Alta/Media/Baja) | Prioridad Final |
|--------------|-------------------------------------|--------------------------------------|----------------|
| Req. 1 | Alto | Alta | Alta |
| Req. 2 | Alto | Alta | Alta |
| Req. 3 | Alto | Media | Alta |

---

### 5.2 Justificación de prioridades

- **Requerimiento 1:** Impacta directamente en la productividad diaria de todos los empleados.  
- **Requerimiento 2:** Compromete la integridad de la información, elemento crítico para la empresa.  
- **Requerimiento 3:** Afecta la continuidad del negocio y atención a clientes.  

---

## 6. Análisis básico de infraestructura

### 6.1 Requerimientos analizados (alta prioridad)

- Requerimiento 1  
- Requerimiento 2  

---

### 6.2 Recursos de infraestructura involucrados

#### Requerimiento 1
- Procesamiento: Capacidad suficiente para múltiples usuarios concurrentes.  
- Memoria: RAM adecuada para evitar saturación.  
- Almacenamiento: Acceso rápido a datos.  
- Red: Ancho de banda suficiente y baja latencia.  

#### Requerimiento 2
- Procesamiento: Control adecuado de accesos y escritura de archivos.  
- Memoria: Soporte estable para operaciones simultáneas.  
- Almacenamiento: Sistema confiable para evitar corrupción o pérdida de datos.  
- Red: Conexión estable para evitar interrupciones durante guardado de archivos.  

---

### 6.3 Riesgos técnicos y puntos únicos de falla (SPOF)

| Requerimiento | Riesgo identificado | Posible SPOF | Justificación |
|--------------|--------------------|--------------|---------------|
| Req. 1 | Saturación del servidor | Servidor único sin redundancia | Si el servidor falla, todos los usuarios quedan sin servicio. |
| Req. 2 | Pérdida total de información | Disco único sin respaldo | La falla del almacenamiento implicaría pérdida completa de datos. |