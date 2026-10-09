> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Logs](section_3.md) ***||*** [Siguiente sección: Seguridad — Vulnerabilidades y Postura](section_5.md)

# Contenido

[[_TOC_]]

# 04 Trazas — Distributed Traces & Service Analysis

## Objetivo: Diagnóstico de servicios mediante trazas distribuidas

Esta sección evaluará la capacidad de los participantes para navegar y analizar trazas distribuidas en Dynatrace. En sistemas de microservicios modernos, las trazas distribuidas son el instrumento clave para diagnosticar degradaciones de rendimiento, identificar queries lentos de base de datos, rastrear excepciones a través de múltiples servicios y localizar el origen exacto de una falla o desperfecto.

Dynatrace captura automáticamente trazas end-to-end a través de toda la cadena de servicios, sin necesidad de instrumentación manual. El análisis de **Distributed Traces**, el **Service Map**, las vistas de **Database Queries** y el **Live Debugger** permiten a los ingenieros pasar de "hay un error" a "línea 200 del archivo Controller.java" en minutos.

Esta sección pondrá a prueba la capacidad de navegar estas herramientas de forma sistemática para responder preguntas concretas de diagnóstico y rendimiento.

---

### Acceso al entorno

Naveguen a **Dynatrace > Applications & Microservices > Distributed Traces** o accedan directamente desde el **Service Map** para explorar los servicios y sus trazas. Para las preguntas de Live Debugger, accede a **Dynatrace > Live Debugger**.

**Código de categoría CTFd**: `2300`  
**Proceso**: `Servicios`  
**Puntos por pregunta**: 45 pts (15 pts × complejidad 3)

---

### Categoría 2300: Trazas

---

#### Pregunta 2301 — Tiempo de respuesta promedio de account ControllerV2

**Descripción**:  
Analicen el servicio Account ControllerV2 y determinen cuál fue su tiempo promedio de respuesta durante los últimos 7 días. Expresen la respuesta en milisegundos (ms).

**Intentos máximos**: 2

---

#### Pregunta 2302 — Cantidad promedio de requests de AdService

**Descripción**:  
Analicen el servicio AdService y determinen cuál es la cantidad promedio de solicitudes que envía por minuto. Expresen la respuesta en requests/min. No incluya unidades

**Intentos máximos**: 2

---

#### Pregunta 2303 — Query con mayor acumulación de duración en BrokerService

**Descripción**:  
Analicen el servicio BrokerService y determinen cuál es el query que registra la mayor duración acumulada durante los ultimos 7 dias. Copien el query completo como respuesta. 

**Intentos máximos**: 2

---

#### Pregunta 2304 — Query más rápido en promedio para OrderController

**Descripción**:  
Analicen el servicio OrderController y determinen cuál es el query a la base de datos con el menor tiempo promedio de ejecución durante los ultimos 10 dias. Copien el query completo como respuesta.

**Intentos máximos**: 2

---

#### Pregunta 2305 — Excepción de span en OrderController

**Descripción**:  
Analicen el servicio OrderController y determinen cuál es la excepción a nivel de span que está causando las fallas observadas, use los últimos 5 dias de referencia.

**Intentos máximos**: 2

---

#### Pregunta 2306 — Mensaje de la excepción en la traza de OrderController

**Descripción**:  
Continúen analizando la falla del servicio OrderController, accedan a la traza asociada e identifiquen el exception class.  


**Intentos máximos**: 2

---

#### Pregunta 2307 — Clase y línea del error en el Stacktrace

**Descripción**:  
Busquen la excepción java.lang.ArithmeticException, analicen el stack trace asociado e identifiquen la clase y la línea de código en la que se produce el error. Respondan utilizando el formato Clase:Línea.

**Intentos máximos**: 2

---

#### Pregunta 2308 — Namespace de la base de datos en la traza

**Descripción**:  
Utilizando la misma traza, identifiquen el namespace de la base de datos con la que se establece la conexión.

**Intentos máximos**: 2

---

#### Pregunta 2309 — Parámetro causante del fallo (Live Debugger)

**Descripción**:  
  Para la misma traza previa, que Db operation name se usa para la interaccion con la base de datos.


**Intentos máximos**: 2

---

## Verificación

Antes de pasar a la siguiente sección, confirmen que han completado:

* [ ] Tiempo de respuesta promedio de Account ControllerV2 en milisegundos.
* [ ] Request rate promedio de AdService en req/min.
* [ ] Query con mayor acumulación de duración en BrokerService.
* [ ] Query más rápido en promedio para OrderController.
* [ ] Excepción de span en OrderController.
* [ ] Mensaje completo de la excepción en la traza de OrderController.
* [ ] Clase y línea exacta del error en el stacktrace.
* [ ] Namespace de la base de datos en la traza.
* [ ] Db operation name usado en la interacción.

> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Logs](section_3.md) ***||*** [Siguiente sección: Seguridad — Vulnerabilidades y Postura](section_5.md)
