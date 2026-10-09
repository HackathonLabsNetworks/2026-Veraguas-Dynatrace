> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Introducción](section_1.md) ***||*** [Siguiente sección: Logs — Log Analytics](section_3.md)

# Contenido

[[_TOC_]]

# 02 Infraestructura — Kubernetes Cluster Analysis

## Objetivo: Dominando la visibilidad sobre infraestructura Kubernetes con Dynatrace

Esta sección evaluará la capacidad de los participantes para navegar y extraer información clave de un entorno Kubernetes monitorizado con Dynatrace. En ambientes de producción reales, los equipos de plataforma necesitan responder rápidamente preguntas sobre el estado de sus clústeres, namespaces, workloads y la configuración de sus pods.

Dynatrace proporciona visibilidad automática y completa sobre Kubernetes sin necesidad de instrumentación manual. **Kubernetes Explorer** ofrece una vista unificada que va desde el clúster hasta el contenedor individual, mostrando versiones, estados de salud, eventos, métricas de recursos y configuraciones de deployments.

Dominar esta vista es fundamental para cualquier SRE o ingeniero de plataforma que necesite diagnosticar problemas de infraestructura tecnológica, planificar capacidad o responder auditorías de configuración de forma ágil y precisa.

---

### Acceso al entorno

Naveguen a **Dynatrace > Infrastructure > Kubernetes** para acceder al Kubernetes Explorer y responder las preguntas de esta sección. Asegúrense de seleccionar el clúster correcto y explorar los namespaces, workloads y pods disponibles.

---

### Categoría 2100: Infraestructura tecnológica

**Código de categoría CTFd**: `2100`  
**Proceso**: `Infra`  
**Puntos por pregunta**: 45 pts (15 pts × complejidad 3)

---

#### Pregunta 2101 — Versión del clúster

**Descripción**:  
Identifiquen cuál es la versión del clúster de Kubernetes que se encuentra monitoreada


**Intentos máximos**: 2

---

#### Pregunta 2102 — Namespace con eventos de backoff

**Descripción**:  
Analicen los datos y determinen qué namespace presenta eventos asociados a backoff


**Intentos máximos**: 2

---

#### Pregunta 2103 — Pods en el namespace kube-system

**Descripción**:  
Analicen los datos y determinen cuántos pods se encuentran corriendo en el namespace kube-system


**Intentos máximos**: 2

---

#### Pregunta 2104 — Contenedor con fallas en namespace Unguard

**Descripción**:  
Analicen los datos y determinen qué contenedor está registrando reinicios dentro del namespace unguard


**Intentos máximos**: 2

---

#### Pregunta 2105 — Límite de CPU del workload Broker-Service

**Descripción**:  
Analicen la configuración del workload broker-service de easytrade y determinen cuál es la cantidad de CPU definida como límite para sus pods


**Intentos máximos**: 2

---

#### Pregunta 2106 — ContainerPort del deployment Unguard-Frontend

**Descripción**:  
Analicen la configuración del deployment unguard-frontend y determinen cuál es el containerPort configurado

**Intentos máximos**: 2

---

#### Pregunta 2107 — Servicio con fallas en pod Unguard-Frontend

**Descripción**:  
Analicen la información disponible y determinen cuál es el servicio que presenta fallas dentro del pod credit-card-order-service.

**Intentos máximos**: 2

---

#### Pregunta 2108 — Ubicación del Centro de Datos del clúster

**Descripción**:  
Analicen la información disponible y determinen cuál es el DynaKube mode con el que se encuentra corriendo el clúster.

**Intentos máximos**: 2

---

#### Pregunta 2109 — Sistema operativo de los nodos

**Descripción**:  
Analicen la información disponible y determinen cuál es el sistema operativo con el que están corriendo los nodos del clúster.


**Intentos máximos**: 2

---

#### Pregunta 2110 — Tipo de instancia de los nodos

**Descripción**:  
Analicen la información disponible y determinen cuál es el tipo de instancia que se está utilizando para los nodos


**Intentos máximos**: 2

---

## Verificación

Antes de pasar a la siguiente sección, confirmen que han completado:

* [ ] Identificada la versión del clúster Kubernetes.
* [ ] Identificado el namespace con eventos de backoff.
* [ ] Contados los pods corriendo en el namespace kube-system.
* [ ] Identificado el contenedor con reinicios en unguard.
* [ ] Revisada la configuración de CPU del workload broker-service.
* [ ] Identificado el containerPort del deployment unguard-frontend.
* [ ] Identificado el servicio con fallas en el pod credit-card-order-service.
* [ ] Localizado el DynaKube mode con el que se encuentra corriendo el clúster.
* [ ] Identificado el sistema operativo de los nodos.
* [ ] Identificado el tipo de instancia de los nodos.

> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Introducción](section_1.md) ***||*** [Siguiente sección: Logs — Log Analytics](section_3.md)
