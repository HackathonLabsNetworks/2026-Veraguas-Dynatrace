> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Seguridad](section_5.md)

# Contenido

[[_TOC_]]

# 06 Experiencia de usuario — Digital Experience Monitoring (DEM)

## Objetivo: Análisis de la experiencia Digital del usuario con Dynatrace RUM

Esta sección final evaluará la capacidad de los participantes para analizar la experiencia del usuario final utilizando las capacidades de **Real User Monitoring (RUM)** y **Digital Experience Monitoring (DEM)** de Dynatrace. En los negocios digitales modernos, la experiencia del usuario es un diferenciador competitivo crítico: entender cómo los usuarios interactúan con las aplicaciones, desde qué geografías, con qué browsers y dónde encuentran errores, es fundamental para la toma de decisiones de producto y operaciones.

Dynatrace DEM captura automáticamente cada sesión de usuario, acción, error de JavaScript, métricas de rendimiento (Apdex, tiempos de carga, Visually Complete) y permite correlacionar la experiencia del frontend con el comportamiento del backend. Los **Business Flows** y los dashboards de análisis de negocio permiten medir el impacto de incidentes técnicos en los KPIs de negocio.

Esta sección pondrá a prueba la capacidad de navegar estas herramientas para obtener insights accionables sobre el comportamiento real de los usuarios en producción.

---

### Acceso al entorno

Naveguen a **Dynatrace > Digital Experience > Web Applications** para acceder a la aplicación **easytrade**. Para las sesiones de usuario individuales, utilicen **Session Replay / Session Segmentation**. Para Business Analytics, accedan a los dashboards vinculados en cada reto.

**Código de categoría CTFd**: `2500`  
**Proceso**: `DEM`  
**Puntos por pregunta**: 60 pts (15 pts × complejidad 4)

---

### Categoría 2500: Experiencia de usuario

---

#### Pregunta 2501 — Browser más utilizado

**Descripción**:  
Analicen la aplicación easytrade y determinen cuál es el navegador más utilizado por los usuarios para acceder a la aplicación.

**Intentos máximos**: 2

---

#### Pregunta 2502 — País con mejor apdex

**Descripción**:  
Analicen el aplicativo y determinen cuál es el país que presenta el mejor índice Apdex en los últimos 30 dias.

**Intentos máximos**: 2

---

#### Pregunta 2503 — País con mayor cantidad de errores

**Descripción**:  
Analicen los datos del aplicativo y determinen cuál es el país que registra la mayor cantidad de errores en los últimos 30 dias.

**Intentos máximos**: 2

---

#### Pregunta 2504 — Excepción frontend más frecuente

**Descripción**:  
Analicen los datos del aplicativo y determinen cuál es la excepción de frontend que se presenta con mayor frecuencia, use la app Error Inspector.

**Intentos máximos**: 2

---

#### Pregunta 2505 — ISP con mayor cantidad de sesiones

**Descripción**:  
Analicen los datos del aplicativo y determinen cuál es el proveedor que registra la mayor cantidad de sesiones.

**Intentos máximos**: 2

---

#### Pregunta 2506 — Tiempo Visually Complete del Login

**Descripción**:  
Analicen el rendimiento del aplicativo y determinen cuál es el tiempo de Visually Complete para la acción 'loading of page/login'. Expresen la respuesta en segundos, no incluyan las unidades.

**Intentos máximos**: 2

---

#### Pregunta 2507 — Acción con fallas para usuario Jessica

**Descripción**:  
Analicen las sesiones de usuario, identifiquen al usuario 'Jessica' y determinen en qué acción presenta fallas.

**Intentos máximos**: 2

---

#### Pregunta 2508 — Ubicación de conexión del usuario Catherine

**Descripción**:  
Analicen las sesiones de usuario, identifiquen a la usuaria 'Catherine' y determinen desde qué ubicación se conecta.

**Intentos máximos**: 2

---

#### Pregunta 2509 — Paso del Business Flow con fallas

**Descripción**:  
Analicen el business flow 'Airline Ticket Booking Flow' y determinen cuál es el paso que presenta fallas.

**Intentos máximos**: 2

---

#### Pregunta 2510 — Excepción de negocio en el Business Flow

**Descripción**:  
Analicen el paso identificado en el business flow y determinen cuál es el event.type que esta generando la excepcion de negocio en este paso.  


**Intentos máximos**: 2

---

#### Pregunta 2511 — Ruta con más Bookings (Dashboard)

**Descripción**:  
Analicen el dashboard del siguiente enlace (https://daa00609.apps.dynatrace.com/ui/document/v0/#share=9a383d3e-2a97-46c1-9e80-cff231eae88d) y determinen cuál es la ruta que generó la mayor cantidad de bookings durante los últimos 7 días. Escriban la respuesta utilizando el formato MEX-PTY.

**Intentos máximos**: 2

---

#### Pregunta 2512 — Pasarela de pago con más fallas

**Descripción**:  
Analicen los datos disponibles y determinen cuál es la pasarela de pago que registra la mayor cantidad de fallas.

**Intentos máximos**: 2

---

#### Pregunta 2513 — Aerolínea con más tickets vendidos

**Descripción**:  
Analicen los datos disponibles y determinen cuál es la aerolínea que registra la mayor cantidad de tickets vendidos.

**Intentos máximos**: 2

---

## Verificación

¡Muchas felicidades por haber completado el reto Dynatrace — Veraguas! Confirmen que han respondido todos los retos de esta sección:

* [ ] Browser más utilizado identificado.
* [ ] País con mejor Apdex identificado.
* [ ] País con mayor cantidad de errores identificado.
* [ ] Excepción frontend más frecuente identificada.
* [ ] ISP con mayor cantidad de sesiones identificado.
* [ ] Tiempo Visually Complete del login obtenido.
* [ ] Acción con fallas del usuario Jessica identificada.
* [ ] Ubicación de conexión de Catherine confirmada.
* [ ] Paso del Business Flow con fallas identificado.
* [ ] Excepción de negocio del Business Flow identificada.
* [ ] Ruta con más bookings del dashboard identificada.
* [ ] Pasarela de pago con más fallas identificada.
* [ ] Aerolínea con más tickets vendidos identificada.

---

## Resumen del Reto — Veraguas

| Categoría | Preguntas Completadas | Puntos Máximos |
|---|---|---|
| Infraestructura | 10 | 450 |
| Logs (PaymentService + Nginx + Network) | 26 | 2,600 |
| Trazas | 9 | 405 |
| Seguridad | 6 | 270 |
| Experiencia de Usuario | 13 | 780 |
| **Total** | **64** | **4,505** |

> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Seguridad](section_5.md)
