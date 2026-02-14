# Práctica 1 - Identificación de necesidades del usuario  

**Unidad 1: Análisis de requerimientos de servidores**  
**Asignatura:** IFS0 - Analizando Necesidades de Infraestructura de Servidores  

---

## 1. Integrantes del grupo
- Nombre completo - Carnet  
- Nombre completo - Carnet  
- Nombre completo - Carnet  

---

## 2. Introducción del caso

Una empresa con **25 empleados** presenta problemas de:
- Lentitud en el sistema  
- Pérdida de archivos  
- Caídas frecuentes del sistema  

No existe documentación técnica formal y los usuarios describen los inconvenientes desde una perspectiva operativa, no técnica.  

El rol asumido es el de **analista de infraestructura**, cuyo objetivo es identificar y estructurar las necesidades del usuario para posteriormente convertirlas en requerimientos claros.

---

## 3. Identificación de necesidades del usuario  

### 3.1 Tabla de necesidades  

| Necesidad | Tipo (Explícita / Implícita) | Clasificación (Operativa / Técnica) | Justificación |
|-----------|------------------------------|-------------------------------------|---------------|
| Mejorar la velocidad del sistema | Explícita | Operativa | Los usuarios reportan lentitud directa en el uso diario del sistema. |
| Evitar pérdida de archivos | Explícita | Operativa | Se reporta pérdida de información que afecta la continuidad del trabajo. |
| Garantizar disponibilidad del sistema | Explícita | Operativa | Las caídas frecuentes interrumpen las actividades laborales. |
| Contar con respaldo de información | Implícita | Técnica | La pérdida de archivos sugiere ausencia o falla en mecanismos de respaldo. |
| Disponer de documentación técnica | Implícita | Técnica | La falta de documentación dificulta el mantenimiento y la gestión del sistema. |

---

## 4. Formulación de requerimientos iniciales  

### 4.1 Tabla de requerimientos  

| Requerimiento inicial | Necesidad relacionada | Clasificación (Funcional / No funcional) | Justificación |
|----------------------|-----------------------|-------------------------------------------|---------------|
| El sistema debe permitir tiempos de respuesta adecuados para 25 usuarios simultáneos | Mejorar la velocidad del sistema | No funcional | Se refiere al rendimiento y desempeño del sistema. |
| El sistema debe garantizar disponibilidad durante la jornada laboral | Garantizar disponibilidad del sistema | No funcional | Está relacionado con niveles de servicio y continuidad. |
| El sistema debe contar con un mecanismo formal de respaldo de información | Evitar pérdida de archivos | Funcional | Define una función específica que el sistema debe cumplir. |
| La infraestructura debe estar documentada | Disponer de documentación técnica | No funcional | Facilita mantenimiento, soporte y escalamiento. |

---

## 5. Observaciones finales  

Las necesidades identificadas son principalmente operativas, pero reflejan posibles deficiencias técnicas en la infraestructura y gestión del sistema.  

En esta etapa no se proponen soluciones técnicas, sino que se estructuran las necesidades para su posterior análisis y diseño de infraestructura.
