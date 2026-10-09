> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Infraestructura](section_2.md) ***||*** [Siguiente sección: Trazas — Distributed Traces](section_4.md)

# Contenido

[[_TOC_]]

# 03 Logs — Log Analytics con DQL

## Objetivo: Investigación forense de logs con Dynatrace Query Language

Esta sección evaluará la capacidad de los participantes para analizar grandes volúmenes de logs usando el **Dynatrace Query Language (DQL)**. En entornos de producción reales, los equipos de ingeniería deben ser capaces de investigar incidentes, auditar transacciones, detectar anomalías de seguridad y cuantificar el impacto de negocio a partir de logs estructurados y semiestructurados.

Dynatrace Log Analytics permite explorar logs de manera interactiva con comandos DQL como `search`, `filter`, `parse`, `summarize`, `sort`, `limit`, `expand`, `fieldsAdd`, y `lookup`. Dominar estas herramientas es esencial para responder preguntas de negocio precisas a partir de datos de logs en tiempo real.

Esta sección está dividida en tres sub-categorías: análisis de logs del servicio **PaymentService**, análisis de logs de acceso **Nginx** y análisis de tráfico de **red**.

---

## Sub-categoría 1: PaymentService logs

### Contexto

El equipo de Operaciones necesita analizar los logs de PaymentService para entender el comportamiento de las transacciones fallidas, calcular métricas de negocio y responder a reportes de usuarios con problemas de pago. Accede al template DQL provisto en el enlace de cada reto.

**Código de categoría CTFd**: `2200`  
**Proceso**: `paymentservice`  
**Puntos por pregunta**: 100 pts (20 pts × complejidad 5)

---

#### Pregunta 2201 — Total de logs con falla en PaymentService

**Descripción**:  
Accedan al siguiente enlace (https://daa00609.apps.dynatrace.com/ui/document/v0/#share=e19edbf8-5baa-478c-a6ac-27ba64203c86) realice una copia, utilicen el template proporcionado y determinen cuántos logs contienen la palabra 'FAIL' asociada a fallas en transacciones del servicio PaymentService.


**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2202 — Código de error más frecuente

**Descripción**:  
Analicen los logs y determinen cuál es el código de error que ocurre con mayor frecuencia.

**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 3

---

#### Pregunta 2203 — Devoluciones exitosamente validadas

**Descripción**:  
Analicen los datos y determinen cuántas devoluciones fueron validadas exitosamente.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2204 — Importe medio reembolsado

**Descripción**:  
Analicen los datos y determinen cuál fue el importe promedio reembolsado.

**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 3

---

#### Pregunta 2205 — Revenue de pagos exitosos validados

**Descripción**:  
Analicen los datos y determinen cuánto revenue fue generado por los pagos validados exitosamente.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2206 — Total de usuarios en el sistema

**Descripción**:  
Analicen la tabla lookup y determinen cuántos usuarios hay en el sistema.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2207 — Diagnóstico de usuaria: Margaret Wilson

**Descripción**:  
Analicen la información disponible sobre la usuaria Margaret Wilson quien se quejó en redes sociales por no haber podido realizar una compra, por lo que determinen qué ocurrió durante su intento de compra y cuál fue la causa del error en el proceso de pago.


**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2208 — Auditoría de transacciones con ID inválido

**Descripción**:  
Analicen las transacciones que presentan el error 'invalid transaction id' durante la fase de validación y determinen si la siguiente afirmación es correcta:

'Existen 10 transacciones que requieren auditoría y seguimiento manual, incluida la transacción con ID fa28b512-54ff-418e-8d9e-1c2fa6465bc7.'


**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 3

---

#### Pregunta 2209 — Transacciones Diamond con problemas técnicos

**Descripción**:  
Analicen los datos y determinen cuántas transacciones realizadas por miembros Diamond fallaron debido a problemas técnicos (códigos de error que comienzan con '50').

**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 3

---

#### Pregunta 2210 — Revenue potencial perdido (Clientes Diamond)

**Descripción**:  
Basándose en los resultados de la pregunta anterior, determinen cuánto revenue potencial se perdió debido a las transacciones fallidas de los miembros Diamond.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

## Sub-categoría 2: Nginx access logs

### Contexto

Los equipos de Seguridad Informática y Operaciones Digitales necesitan analizar los logs de acceso del servidor Nginx para detectar patrones de tráfico, problemas de compatibilidad de browsers en dispositivos móviles, tráfico geográfico sospechoso y posibles intentos de explotación de vulnerabilidades conocidas como CVE-2019-11043.

**Código de categoría CTFd**: `2200`  
**Proceso**: `nginx access`  
**Puntos por pregunta**: 100 pts (20 pts × complejidad 5)

---

#### Pregunta 2211 — Registros con método HTTP POST

**Descripción**:  
Accedan al siguiente enlace (https://daa00609.apps.dynatrace.com/ui/document/v0/#share=52641ddc-0874-4fa5-a8b1-f39fa4168174) realice una copia, utilicen el template proporcionado y determinen cuántos registros del log de acceso utilizan el método HTTP POST

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2212 — Tamaño medio de respuestas

**Descripción**:  
Determinen cuál es el tamaño promedio de las respuestas registradas en los logs de acceso.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2213 — Accesos a Broker-Service desde Chrome en Android antiguo

**Descripción**:  
Analicen los registros del log de acceso y determinen cuántas solicitudes a las URL de broker-service fueron realizadas desde navegadores Chrome en dispositivos Android con una versión del sistema operativo inferior a la 10.0.


**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2214 — Solicitudes desde Estados Unidos

**Descripción**:  
Analicen todos los registros del log de acceso y determinen cuántas solicitudes se originaron en Estados Unidos.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2215 — Tráfico sospechoso CVE-2019-11043

**Descripción**:  
Analicen los registros de acceso y determinen desde qué ciudad se originó el tráfico sospechoso asociado a un posible intento de explotación de la vulnerabilidad CVE-2019-11043.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2216 — Accesos a la página raíz /

**Descripción**:  
Analicen los registros de acceso y determinen cuántas veces se accedió a la página raíz (/).

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2217 — Tercera IP con más tráfico

**Descripción**:  
Analicen los registros de tráfico y determinen cuál es la tercera dirección IP que genera el mayor volumen de tráfico.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

## Sub-categoría 3: Network logs

### Contexto

El equipo de Seguridad Informática necesita analizar el tráfico de red capturado para entender el comportamiento de las aplicaciones, detectar actividad anómala, identificar servidores con cifrado débil y descubrir actividad de aplicaciones prohibidas (P2P y minería de criptomonedas). Este dataset de red es de mayor volumen que el de Panamá, con más aplicaciones, orígenes y destinos distintos.

**Código de categoría CTFd**: `2200`  
**Proceso**: `network`  
**Puntos por pregunta**: 100 pts (20 pts × complejidad 5)

---

#### Pregunta 2218 — Aplicaciones distintas en el tráfico de red

**Descripción**:  
Accedan al siguiente enlace (https://daa00609.apps.dynatrace.com/ui/document/v0/#share=45ac0f0c-9218-481f-8478-02daa3277df0) realice una copia, utilicen el template proporcionado y determinen cuántas aplicaciones diferentes fueron observadas en el tráfico de red.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2219 — Orígenes distintos en el tráfico de red

**Descripción**:  
Determinen cuántos orígenes diferentes fueron observados en el tráfico de red.

**Intentos máximos**: 2

---

#### Pregunta 2220 — Destinos distintos en el tráfico de red

**Descripción**:  
Determinen cuántos destinos diferentes fueron observados en el tráfico de red.

**Intentos máximos**: 2

---

#### Pregunta 2221 — Top 3 Apps por TCP Round-Trip-Time

**Descripción**:  
Determinen cuáles son las tres aplicaciones con el mayor promedio de TCP round-trip time (RTT). Escriban su respuesta separando las aplicaciones por comas.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2222 — Aplicaciones personales del Ingeniero de Nube

**Descripción**:  
Analicen la actividad de red asociada a la dirección IP 172.16.133.66 y determinen cuántas aplicaciones de uso personal ha utilizado el Ingeniero de Nube debido a las evidencias de baja productividad.

**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

#### Pregunta 2223 — Bytes de tráfico del Ingeniero de Nube

**Descripción**:  
Continuando con la pregunta anterior, analicen la actividad de red asociada a la dirección IP 172.16.133.66 y determinen cuántos bytes de tráfico generó.


**Intentos máximos**: 2

---

#### Pregunta 2224 — IPs de servidores con cifrado SSL/TLS débil

**Descripción**:  
Con el fin de reforzar la seguridad de la red corporativa, entrará en vigor una nueva política que obligará a que todo el tráfico SSL/TLS utilice un cifrado con una clave de al menos 256 bits, por lo que analicen el tráfico de red y determinen qué servidores con direcciones IP privadas utilizan SSL/TLS con claves de cifrado inferiores a 256 bits. Escriban las direcciones IP identificadas separadas por comas. Tip: las IPs de los servidores tienen que ser de tipo privado.


**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 3

---

#### Pregunta 2225 — Ubicación con más tráfico P2P

**Descripción**:  
Analicen el tráfico de red asociado a aplicaciones P2P restringidas (BitTorrent, eDonkey, Kazaa, Gnutella y Ares) y determinen de los dispositivos internos que están generando y recibiendo más tráfico a estas aplicaciones, cuál es la ubicación que registra el mayor volumen total de tráfico (en bytes), considerando tanto el tráfico enviado como el recibido.

**Pista 1** *(costo: 30 pts)*:

**Pista 2** *(costo: 30 pts)*:

**Intentos máximos**: 3

---

#### Pregunta 2226 — ID de activo del nodo de minería de Criptomonedas

**Descripción**:  
La actividad de minería de criptomonedas es delicada y además está prohibida en la red corporativa. Esto incluye aplicaciones como 'bitcoin', 'ethereum', 'ethereum-nd', 'minexmr-com' y 'monero'. La principal amenaza para la seguridad informática es la presencia de nodos de red que muestran tráfico de minería de criptomonedas. Por lo que analicen el tráfico de red e identifiquen los nodos que presentan tráfico de minería de criptomonedas tanto entrante como saliente.Identifique cual es el asset_id que mas veces esta presente. 


**Pista 1** *(costo: 40 pts)*:

**Intentos máximos**: 2

---

## Verificación

Antes de pasar a la siguiente sección, confirmen que han completado:

* [ ] **PaymentService** (10 preguntas): Análisis de transacciones fallidas, revenue, usuarios, diagnóstico de Margaret Wilson.
* [ ] **Nginx access** (7 preguntas): Análisis de tráfico web, Chrome en Android, geo-ubicación, CVE-2019-11043.
* [ ] **Network** (9 preguntas): Aplicaciones P2P, cifrado TLS, ingeniero de nube, minería de criptomonedas.

> ***Ir a***: [Menú principal](../README.md) ***||*** [Anterior: Infraestructura](section_2.md) ***||*** [Siguiente sección: Trazas — Distributed Traces](section_4.md)
