> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Trazas](section_4.md) ***||*** [Siguiente sección: Experiencia de Usuario — DEM](section_6.md)

# Contenido

[[_TOC_]]

# 05 Seguridad — Vulnerabilidades y postura de seguridad

## Objetivo: Evaluación de vulnerabilidades y cumplimiento de seguridad con Dynatrace

Esta sección evaluará la capacidad de los participantes para navegar y analizar las capacidades de **Application Security** de Dynatrace. En entornos de producción modernos, la seguridad no es un proceso separado sino una dimensión continua de la observabilidad: los equipos necesitan detectar CVEs en sus dependencias, evaluar el impacto de vulnerabilidades conocidas sobre sus entidades, y verificar el cumplimiento de posturas de seguridad como los benchmarks CIS y STIGs de Kubernetes.

Dynatrace Application Security proporciona visibilidad automática sobre vulnerabilidades de terceros (software composition analysis), mapea qué entidades están afectadas y ofrece evaluaciones de postura de seguridad contra estándares industriales. Esta integración entre observabilidad y seguridad permite priorizar remediaciones basadas en el impacto real sobre el entorno de producción.

---

### Acceso al entorno

Naveguen a **Dynatrace > Application Security > Vulnerabilities** para las preguntas de CVEs y vulnerabilidades de software. Para las preguntas de postura y STIGs, naveguen a **Dynatrace > Application Security > Security Posture** o la sección equivalente de Kubernetes Security.

**Código de categoría CTFd**: `2400`  
**Proceso**: `Vulnerabilidades`  
**Puntos por pregunta**: 45 pts (15 pts × complejidad 3)

---

### Categoría 2400: Seguridad

---

#### Pregunta 2401 — Componente a corregir para vulnerabilidad S-99

**Descripción**:  
Analicen la vulnerabilidad S-99 y determinen cuál es el componente que debe corregirse para remediarla.


**Intentos máximos**: 2

---

#### Pregunta 2402 — Entidad afectada por CVE-2024-47554

**Descripción**:  
Analicen la vulnerabilidad CVE-2024-47764 y determinen cuál es la entidad afectada por esta vulnerabilidad.

**Intentos máximos**: 2

---

#### Pregunta 2403 — Versión del componente afectado por S-246

**Descripción**:  
Analicen la vulnerabilidad S-246 y determinen cuál es la versión del componente afectado que presenta la vulnerabilidad.

**Intentos máximos**: 2

---

#### Pregunta 2404 — STIG vulnerability ID para componentes obsoletos de Kubernetes

**Descripción**:  
Analicen la vulnerabilidad 'Kubernetes must remove old components after updated versions have been installed' en la app Secure Posture Management y determinen cuál es su STIG Vulnerability ID.

**Intentos máximos**: 2

---

#### Pregunta 2405 — Namespace en cumplimiento para Network Policies

**Descripción**:  
Analicen la postura 'Ensure that all Namespaces have Network Policies defined' en la app Secure Posture Management y determinen cuál es el único namespace que no es relevante.


**Intentos máximos**: 2

---

#### Pregunta 2406 — Namespace resuelto en estado Manual

**Descripción**:  
  Analicen la regla 'Minimize the admission of containers wishing to share the host process ID namespace' en la app Secure Posture Management y determinen cuál es el namespace en estado Manual.

**Intentos máximos**: 2

---

## Verificación

Antes de pasar a la siguiente sección, confirmen que han completado:

* [ ] Identificado el componente a corregir para la vulnerabilidad S-99.
* [ ] Identificada la entidad afectada por CVE-2024-47764.
* [ ] Encontrada la versión del componente vulnerable en S-246.
* [ ] Localizado el STIG Vulnerability ID para remoción de componentes obsoletos.
* [ ] Identificado el namespace en cumplimiento para Network Policies.
* [ ] Identificado el namespace resuelto en estado Manual.

> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Trazas](section_4.md) ***||*** [Siguiente sección: Experiencia de Usuario — DEM](section_6.md)
